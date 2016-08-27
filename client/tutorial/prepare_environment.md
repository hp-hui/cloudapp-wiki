### 准备环境
#### 安装Git
1. 下载

  可在 https://git-scm.com/download 下载到OS X, Windows, Linux等各个平台的安装包。
2. 安装

OS        | 方法
--------- | --------
OS X      | 打开下载的git磁盘镜像文件(文件名后缀是.dmg),即可安装。
Windows   | 打开下载的git安装程序，即可安装。
Ubuntu    |`apt-get install git`

#### 安装CocoaPods
 1. 移除现有的Ruby默认源
 ```shell
 $gem sources --remove https://rubygems.org/
 ```
 2. 使用新的源
 ```shell
 $gem sources -a https://ruby.taobao.org/
  ```
 3. 验证新源是否替换成功
  ```shell
  $gem sources -l
   ```
 4. 安装CocoaPods
 ```shell
 $sudo gem install cocoapods
 $pod setup
  ```
  5.更新gem
  ```shell
  $sudo gem update --system
  ```

#### 安装开发工具XCode ( iOS SDK)
 1. 进入`App Store`
 2. 搜索`Xcode`
 3. 点击`Free`按钮，然后点击`Install App`

#### 安装JDK
Operating System | Min JDK Version | Max JDK Version | Package Arch Version | Download Location | Notes
--------- | -------- | --------- | -------- | --------- | --------
OS X |6 | 8 latest revision |64-bit | [Official Website](http://www.oracle.com/technetwork/java/javase/downloads/index.html) |On Mac OS X 10.6 (Snow Leopard) and earlier, the JDK is preinstalled. - On Mac OS X 10.7 (Lion) and later, the OS should prompt you to install it when needed.Android Development on OS X systems requires Java 6 runtime to be installed.
Windows | 7 | 8 latest revision | 32-bit only (x86 / i586) | [Official Website](http://www.oracle.com/technetwork/java/javase/downloads/index.html)|The 32-bit version of the JDK is required regardless of whether Titanium is running on a 32-bit or 64-bit Windows system.Studio offers to install JDK 7 if no JDK is found.
#### 安装Android Studio
 1. 下载
  - 安装版 http://developer.android.com/sdk/index.html
  - 绿色版 http://tools.android.com/recent
 2. 使用安装版安装Android Studio
   1. 执行android-studio-bundle-143.2915827-windows.exe，可以看到欢迎页
   2. 在选择安装组件中，虚拟机可以不用安装
   3. 接下就一直Next直到安装完成

#### 安装Android SDK
使用"安装版"安装的Android Studio已经默认安装Android SDK。若未安装，需先下载Android SDK,并设置Android SDK安装路径到Android Studio中。
 1. 下载: https://dl.google.com/android/android-sdk_r24.4.1-windows.zip
 2. 解压zip包，并执行SDK Manager
 3. 一路安装下去即可。
