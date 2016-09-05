## restrpc

Service side
```lua
local restrpc = require "framework.restrpc"

local function calc(a, b)
    return a + b, a - b
end

function onReady()
    restrpc.start({
        ["calc"] = calc
    }, true)
end
```

Caller side
```lua
local service = restrpc.new(<service-appid>)
local result1,result2 = service.calc(100, 200)
-- result1 = 300, result2 = -100
```
