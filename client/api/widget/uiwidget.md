## uiwidget

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| id | string | readonly |
| alpha | number | widget alpha |
| transform | table | use affine lib to create transform table |
| touchDisabled | boolean | disable touch |
| hidden | boolean | |
| onchange | function | |
| onerror | function | |
| onload | function | |
| ontouchup | function | |
| ontouchdown | function | |
| ontouchmove | function | |
| backgroundAlpha | number | |
| backgroundColor | color:[ColorType] | |
| backgroundGradient | gradient:[GradientType] | |
| backgroundImage | image:[ImageType] | |
| backgroundScale | scale:[ScaleType] | |
| borderColor | color:[ColorType] | |
| borderAlpha | number | |
| borderWidth | number | |
| cornerRadius | number | |
| width | size:[SizeType] | |
| height | size:[SizeType] | |
| marginLeft | size:[SizeType] | |
| marginRight | size:[SizeType] | |
| marginTop | size:[SizeType] | |
| marginBottom | size:[SizeType] | |
| margin | string | top,right,bottom,left |
| paddingLeft | size:[SizeType] | |
| paddingRight | size:[SizeType] | |
| paddingTop | size:[SizeType] | |
| paddingBottom | size:[SizeType] | |
| padding | string | top,right,bottom,left |

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| mark | void | void | save widget current status |
| reset | void | void | reset widget status by status saved before. |
| suspendLayout | void | void | suspend layout in order to do layout transaction. |
| resumeLayout | duration:float = 0, oncomplete:function = nil | void | commit layout changes |
| getSnapshot | void | img:[LuaImage] | take snapshot of this widget |
| getContentSnapshot | void | img:[LuaImage] | take content snapshot of this widget |
| getRect | void | x:number,y:number,width:number,height:number | 	get the rect of this widget |
| getMarginOnView | widget:[uiwidget] | top:number,right:number,bottom:number,left:number | |
| getRectOnView | widget:[uiwidget] | x:number,y:number,width:number,height:number | |
| setStyle | styles:table | void | merge style table |
