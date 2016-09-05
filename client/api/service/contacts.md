## contacts

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| load | func:LuaFunction | void | load contacts, func will be invoked on complete |
| addChangeWatcher | func:LuaFunction | LuaFunctionWatcher | func will be invoked on contacts changes. |
| getAll | void | List | get all contacts List, item in list: LuaRecord |

### Samples
```lua
local contactsService = registry.getService("contacts")
local watcher = contactsService:addChangeWatcher(function(...)
	print(...)
end)
contactsService:load(function(cs, success)
	print(cs, success)
	for i,v in ipairs(cs.all) do
		for i2,v2 in pairs(v) do
			print(i2,v2)
		end
		print(i,v.fullName, json.encode(v.phones))
	end
end)
```
