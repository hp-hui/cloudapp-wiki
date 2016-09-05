## location

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| addLocationWatcher | func:LuaFunction | watcher:LuaFunctionWatcher | add location watcher, will be called when location changes. callback(location:LuaLocation) |
| addHeadingWatcher | func:LuaFunction | watcher:LuaFunctionWatcher | add heading watcher, will be called when heading changes. callback(heading:LuaHeading) |
| start | void | result:boolean | start location service |
| stop | void | result:boolean | stop location service |
| newLocation | latitude:number,longitude:number | location:LuaLocation | create a new LuaLocation Object |
