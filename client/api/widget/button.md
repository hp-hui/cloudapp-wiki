## button extends [uiwidget](uiwidget.md)

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| label | string | button text label |
| onclick | string/function | button onclick script |
| color | string/number | button label color |
| fontName | string | button label fontName |
| fontSize | number | button label fontSize |
| bold | boolean | button label bold |
| underline | boolean | button label underline |
| align | string | left,center,right |
| showsTouch | boolean | |
| showsTouchWhenHighlighted | boolean | ios only |
| exclusiveTouch | boolean | ios only |
| onmousedown | function | button onmousedown |
| onmouseup | function | button onmouseup |

### xml schema
```xml
<button label="string" color="#123456" align="left|center|right" fontSize="22" bold="true|false" underline="true|false" >
```

### xml sample
```xml
<button text="Say Hi" id="widgetid" height="50"/>
```

### lua sample
<!-- [FILE] sample/scripts/widget/button.lua -->
```lua
widgetid.onclick = function()
    alert("Click on Button")
end
```

### any file demo
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
