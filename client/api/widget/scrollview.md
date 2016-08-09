## scrollview
scrollview container.

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| dragDownLayout | layout | |
| dragDownMinMovement | number | |
| onDragDownStateChanged | function | |
| onDragDownAction | function | |
| pagingEnabled | boolean | ios only |
| decelerationEnabled | boolean | ios only |
| direction | string | android only, vertical / horizontal, default:vertical |
| scrollmodel | string | android only value:hvmodel 和direction属性组合使用。只有在direction="horizontal" 才有效 |

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| setContentOffset | x:number, y:number, animation:boolean(optional) | void | set content offset inside scrollview |
| getContentOffset | void | x:number, y:number | get the content offset. |
| setContentSize | width:number,height:number | void | set the content size, ios only. |
| getContentSize | void | width:number, height:number | get the content size, ios only. |

### callback list
| Property      | Parameters    | Description   |
| ------------- | ------------- | ------------- |
| onchange | scrollview:[ScrollView](scrollview.md), contentOffsetX:number, contentOffsetY:number | callback on scrollview's contentoffset changed. |
| ontouchup | scrollview:[ScrollView](scrollview.md), contentOffsetX:number, contentOffsetY:number | callback when touch up on scrollview. |
| ontouchdown | scrollview:[ScrollView](scrollview.md), contentOffsetX:number, contentOffsetY:number | callback when touch down on scrollview. |
| ontouchmove | scrollview:[ScrollView](scrollview.md), contentOffsetX:number, contentOffsetY:number | callback when touch move on scrollview. |

### xml schema
```xml
<scrollview pagingEnabled="true|false" decelerationEnabled="true|false" >
```

### xml sample
```xml
<scrollview id="widgetid">
  ...
</scrollview>
```

### lua sample
```lua
widgetid.ontouchup = function(sv,x,y)
    print("ontouchup",sv,x,y)
end

widgetid.ontouchdown = function(sv,x,y)
    print("ontouchdown",sv,x,y)
end

widgetid.ontouchmove = function(sv,x,y)
    print("ontouchmove",sv,x,y)
end

widgetid.onchange = function(sv,x,y)
    print("onchange",sv,x,y)
end

widgetid:setContentOffset(100,100)

local w,h = widgetid:getContentSize()
local x,y = widgetid:getContentOffset()
```
