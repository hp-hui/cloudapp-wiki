## storage

```lua
local storage = require "framework.storage"

storage.load(key, scope)
storage.save(key, value, scope, timeout)

scope:
storage.SCOPE_GLOBAL
storage.SCOPE_APP
storage.SCOPE_PAGE
```
