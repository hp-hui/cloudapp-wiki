## view

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| layout | string | absolute / none |
| overflow | string | visible / hidden / scroll |

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| reLayoutChildren | void | void | relayout all child items |
| addChild | child:object, position:number(optional) | child:[UIWidget](uiwidget.md) | add a child model or widget inside this view |
| indexChild | child:object | position:number | find position of a child, child could be id/widget |
| removeChild | child:object | void | remove a child, child could be id/widget |
| removeChildAt | position:number | void | remove a child at position |
| removeAllChildren | void | void | remove all children |
| listChildren | void | children:table | get the list of all children |

### xml schema
```xml
<view layout="absolute|flow-x|flow-y" overflow="visible|hidden|scroll" >
```

### xml sample
```xml
<view width="50" backgroundColor="red">
  <button xxx>
</view>
```
