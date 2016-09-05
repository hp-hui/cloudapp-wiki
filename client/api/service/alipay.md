## alipay
```lua
local alipay = registry.getService("alipay")

local signStr = "xxx"
alipay:pay(signStr, function(ret)
    for k,v in pairs(ret) do
        print(k,v)
    end
end)
```

如果程序从支付宝回来前已经被kill掉，那么在相关业务逻辑读取`$alipay_result`以获得支付结果
```lua
local ret = sandbox:getGlobalSandbox():get("$alipay_result")
if ret then
    -- clear result
    sandbox:getGlobalSandbox():put("$alipay_result", nil)

    for k,v in pairs(ret) do
        print(k,v)
    end
end
```
