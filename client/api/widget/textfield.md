## textfield
single line text input field.

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| password | boolean | |
| editable | boolean | |
| doneable | boolean | |
| maxLength | number | |
| keyboard | string | |
| returnType | string | |
| borderStyle | string | roundrect / line / bezel |
| placeholder | string | |

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| setText | text:string | void | set textfield's text |
| getText | void | string | get textfield's text |
| setFocus | width:number,height:number | void | set the content size, ios only. |
| clearFocus | void | width:number, height:number | get the content size, ios only. |

### callback list
| Property      | Parameters    | Description   |
| ------------- | ------------- | ------------- |
| onReturnClick | void | callback on keyboard return click |
| onDoneClick | void | callback on keyboard done click |
| onblur | void | callback on blur |
| onfocus | void | callback on focus |

### xml schema
```xml
```

### xml sample
```xml
<textfield text="display" align="left" height="50"/>
```

### lua sample
```lua

```
