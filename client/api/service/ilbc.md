## ilbc

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| play | filePath:string | void | |
| startRecord | filePath:string | void | |
| stopRecord | void | void | |

```lua
local ilbc = registry.getService("ilbc")
ilbc:startRecord("data:///record.ilbc")

sleep(5)
ilbc:stopRecord()
sleep(2)
ilbc:play("data:///record.ilbc")
```
