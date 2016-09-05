## keyboard

```lua
Event.gbind("EventKeyKeyBoardRectWillChange", function(e)
    local x,y,width,height = e:getRect()
    print(x,y,width,height)
end, _ENV)
Event.gbind("EventKeyKeyBoardRectChanged", function(e)
    local x,y,width,height = e:getRect()
    print(x,y,width,height)
end, _ENV)
```
