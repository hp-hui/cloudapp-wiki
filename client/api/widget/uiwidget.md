## uiwidget
This the abstract class of all widget.

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
| backgroundColor | color:[ColorType](../common/colortype.md) | |
| backgroundGradient | gradient:[GradientType](../common/gradienttype.md) | |
| backgroundImage | image:[ImageType](../common/imagetype.md) | |
| backgroundScale | scale:[ScaleType](../common/scaletype.md) | |
| borderColor | color:[ColorType](../common/colortype.md) | |
| borderAlpha | number | |
| borderWidth | number | |
| cornerRadius | number | |
| width | size:[SizeType](../common/sizetype.md) | |
| height | size:[SizeType](../common/sizetype.md) | |
| marginLeft | size:[SizeType](../common/sizetype.md) | |
| marginRight | size:[SizeType](../common/sizetype.md) | |
| marginTop | size:[SizeType](../common/sizetype.md) | |
| marginBottom | size:[SizeType](../common/sizetype.md) | |
| margin | string | top,right,bottom,left |
| paddingLeft | size:[SizeType](../common/sizetype.md) | |
| paddingRight | size:[SizeType](../common/sizetype.md) | |
| paddingTop | size:[SizeType](../common/sizetype.md) | |
| paddingBottom | size:[SizeType](../common/sizetype.md) | |
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
| getMarginOnView | widget:[uiwidget](uiwidget.md) | top:number,right:number,bottom:number,left:number | |
| getRectOnView | widget:[uiwidget](uiwidget.md) | x:number,y:number,width:number,height:number | |
| setStyle | styles:table | void | merge style table |
