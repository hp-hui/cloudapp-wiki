## 全局属性

* `sandbox` 不同位置取sandbox得到不同的类型，initialize.lua 里面得到的是AppSandbox, page内得到的是PageSandbox
* `_S` 同一个appId任何地方取_S得到的是共享的一个lua table
* `appId` 任意位置取 sandbox.appId 都可以得到当前appId
* `appVersion` 任意位置取 sandbox.appVersion 都可以得到当前appVersion
