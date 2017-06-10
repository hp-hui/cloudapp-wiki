## view

### 属性
| 属性      | 类型          | 描述   |
| ------------- | ------------- | ------------- |
| layout | string |view的布局 absolute / none |
| overflow | string | visible / view超出部分是否隐藏 hidden / scroll |

### 接口
| 属性      | 参数    | 返回  | 描述   |
| ------------- | ------------- | ------------- | ------------- |
| reLayoutChildren | void | void | 重汇view所有子元素的界面 |
| addChild | child:object, position:number(optional) | child:[UIWidget](uiwidget.md) | 添加一个widget到view里面 |
| indexChild | child:object | position:number | find position of a child, child could be id/widget |
| removeChild | child:object | void | 根据widget或者id移除子元素 |
| removeChildAt | position:number | void | 根据位置移除子元素 |
| removeAllChildren | void | void | 移除view里面所有子元素 |
| listChildren | void | children:table | 获取view里面所有子元素 |

### xml 模板
```xml
<view layout="absolute|flow-x|flow-y" overflow="visible|hidden|scroll" >
```

### xml 样例
```xml
<view width="50" backgroundColor="red">
  <button xxx>
</view>
```
