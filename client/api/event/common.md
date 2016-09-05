## common

### Device Shake
```lua
local Event = require "framework.event"
Event.gbind(Event.DEVICE_SHAKE, function(e)
    print(e)
end, _ENV)
```

### Background,Foreground
```lua
local Event = require "framework.event"
Event.gbind("OnBackground", function()
    print("OnBackgroundOnBackground")
end, _ENV)
Event.gbind("OnForeground", function()
    print("OnForegroundOnForeground")
end, _ENV)
```
