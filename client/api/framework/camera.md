## camera

```lua
local camera = require "framework.camera"
camera.takePhoto{
  camera = true | false | nil,
  allowsEditing = true | false,
  onsuccess=function(img)
    img:getFullScreenImage():save(localFilePath,"jpg")
    ...
  end,
  oncancel=function()
  end
}
```
