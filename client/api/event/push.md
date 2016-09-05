## push

```lua
local utils = require "framework.utils"
local base = require "framework.base"
local Event = require "framework.event"

Event.gbind(Event.PUSH_TOKEN_UPDATED, function(e)
    print(e.token) -- nil on fail
end)

Event.gbind(Event.PUSH_NOTIFICATION, function(e)
    print(e.alert, e.badge, e.body)

    print(base.getGSandbox():get("notification_data")) -- any place you want after app launch.
    base.getGSandbox():put("notification_data", nil) -- clear data
end)

utils.requestPushToken()
```
