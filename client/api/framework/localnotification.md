## localnotification

```lua
local localnotification = require "framework.localnotification"

local t = require "framework.localnotification"
t.clear()
t.add{
    sound = t.defaultSound,
    title = "You have a new message.",
    action = "ClickMe",
    datetime = os.time() + 10, -- 10s later
    body = {id = "0001"} -- any table map.
}

local Event = require "framework.event"
local json = require "json"
Event.gbind(Event.PUSH_NOTIFICATION, function(e)
    print(json.encode(e.body))
end, _ENV)

```
