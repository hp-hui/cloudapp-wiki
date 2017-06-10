## uiwidget
这是所有widget的抽象类

### 属性
| 属性      | 类型          | 描述   |
| ------------- | ------------- | ------------- |
| id | string | 只读唯一标识 |
| alpha | number | widget透明度 |
| transform | table | use affine lib to create transform table |
| touchDisabled | boolean | 是否有点击事件 |
| hidden | boolean | widget是否隐藏 |
| onchange | function | |
| onerror | function |ios独有 |
| onload | function |ios独有 |
| ontouchup | function |widget触碰抬起事件 |
| ontouchdown | function |widget触碰事件 |
| ontouchmove | function |widget触碰移动事件 |
| backgroundAlpha | number | widget背景的透明度 |
| backgroundColor | color:[ColorType](../common/colortype.md) | widget背景颜色|
| backgroundGradient | gradient:[GradientType](../common/gradienttype.md) | |
| backgroundImage | image:[ImageType](../common/imagetype.md) |widget背景图片 |
| backgroundScale | scale:[ScaleType](../common/scaletype.md) |widget背景图片的拉伸 |
| borderColor | color:[ColorType](../common/colortype.md) |widget边框的颜色 |
| borderAlpha | number |widget边框的透明度 |
| borderWidth | number |widget边框的宽度 |
| cornerRadius | number | widget四角的弧度|
| width | size:[SizeType](../common/sizetype.md) |widget的宽度 |
| height | size:[SizeType](../common/sizetype.md) |widget的高度 |
| marginLeft | size:[SizeType](../common/sizetype.md) |widget距离父容器左边的距离 |
| marginRight | size:[SizeType](../common/sizetype.md) |widget距离父容器右边的距离 |
| marginTop | size:[SizeType](../common/sizetype.md) |widget距离父容器顶部的高度 |
| marginBottom | size:[SizeType](../common/sizetype.md) |widget距离父容器底部的高度 |
| margin | string | widget距离父容器 上，右，下，左四个方向的距离 |
| paddingLeft | size:[SizeType](../common/sizetype.md) | widget内部元素距离widget左边的距离 |
| paddingRight | size:[SizeType](../common/sizetype.md) |widget内容元素距离widget右边的距离 |
| paddingTop | size:[SizeType](../common/sizetype.md) |widget内部元素距离widget上方的高度 |
| paddingBottom | size:[SizeType](../common/sizetype.md) |widget内部元素距离widget下方的高度 |
| padding | string | widget内部元素距离widget 上，右，下，左四个方向的距离 |

### 接口
| 属性      | 参数    | 返回   | 描述   |
| ------------- | ------------- | ------------- | ------------- |
| mark | void | void | 保存widget当前的状态 |
| reset | void | void | 重置widget状态恢复到保存的时候|
| suspendLayout | void | void | suspend layout in order to do layout transaction. |
| resumeLayout | duration:float = 0, oncomplete:function = nil | void | commit layout changes |
| getSnapshot | void | img:[LuaImage] | widget截图|
| getContentSnapshot | void | img:[LuaImage] | take content snapshot of this widget |
| getRect | void | x:number,y:number,width:number,height:number | 获取widget在容器内的水平位置和大小 |
| getMarginOnView | widget:[uiwidget](uiwidget.md) | top:number,right:number,bottom:number,left:number | 获取widget在容器上下左右的位置|
| getRectOnView | widget:[uiwidget](uiwidget.md) | x:number,y:number,width:number,height:number | |
| setStyle | styles:table | void | merge style table |
