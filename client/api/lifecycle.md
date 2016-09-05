## 生命周期

### App生命周期
* `onInstalled()` app 首次安装时触发
* `onPatched(oldVersion)` app 被更新后触发
* `onReady()` app 每次启动准备完成后触发

### Page生命周期
* `onCreated(ctx:table)` page 被创建时触发
* `onFronted()` page 位于最顶部时触发
* `onIdle()` page 不再位于最顶部时触发
* `onTap()` page 被点击未处理时触发
* `onSwipeUp()` page 上滑事件触发
* `onSwipeDown()` page 下滑事件触发
* `onSwipeLeft()` page 左滑事件触发
* `onSwipeRight()` page 右滑事件触发
* `onNavBack()` android返回按钮被点击时触发
