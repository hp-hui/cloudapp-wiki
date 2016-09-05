## image

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| load | filePath:string | LuaImage | |

### Samples
```lua
local imageservice = registry.getService("image")
local img = imageservice:load(filePath)
local width,height = img:getSize()
```
