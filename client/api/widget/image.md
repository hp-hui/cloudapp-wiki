## image extends [UIWidget](uiwidget.md)

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| placeholder | [ImageType](../common/imagetype.md) except http | placeholder image before image from remote loaded. |
| scale | string | none / fill / center / fitWidth / fitHeight / clip([0-9]+,[0-9]+(,[0-9]+,[0-9]+)?) |
| src | [ImageType](../common/imagetype.md) | set image source |

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| setImage | image | boolean | set image |
| getImage | void | image | get image |

### xml schema
```xml
<view layout="absolute|flow-x|flow-y" overflow="visible|hidden|scroll" >
```

### xml sample
```xml
<image src="app://login_resources/login_background.jpg" scale="none"/>
```
