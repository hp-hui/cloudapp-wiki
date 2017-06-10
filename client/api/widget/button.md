## button 继承于 [uiwidget](uiwidget.md)

### 属性
| 属性      | 类型          | 描述   |
| ------------- | ------------- | ------------- |
| label | string |  显示文本 |
| onclick | string/function | 点击事件|
| color | string/number | 文本的颜色 |
| fontName | string | 文本字体类型 |
| fontSize | number | 文本字体大小|
| bold | boolean | 文本是否是粗体 |
| underline | boolean |文本是否有下划线 |
| align | string | 文本对其方式  left,center,right |
| showsTouch | int | 0~1 0没有阴影效果 1有阴影效果 |
| showsTouchWhenHighlighted | boolean | ios 独有 |
| exclusiveTouch | boolean | ios 独有 |
| onmousedown | function | 手指按下执行事件 |
| onmouseup | function | 手指起来执行事件  |

### xml 模板
```xml
<button label="string" color="#123456" align="left|center|right" fontSize="22" bold="true|false" underline="true|false" >
```

### xml 样例
```xml
<button text="Say Hi" id="widgetid" height="50"/>
```

### lua 样例
<!-- [FILE] sample/scripts/widget/button.lua -->
```lua
widgetid.onclick = function()
    alert("Click on Button")
end
```

### 文件演示
<!-- [FILE] sample/button.xml -->
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<page>
		<layout>
      		<button text="Say Hi" id="widgetid" height="50"/>
    	</layout>
	</page>
</manifest>
```
