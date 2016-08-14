## 部署服务器

### 目标
* 在Linux或MacOS上部署Cloud App服务器端.

### 前置条件
* Linux / Mac
* JDK 7.0
* Playframework 1.3.x 
* **play**和**java**已经配置进了PATH

### 操作

#### 初始化

假定将服务器端部署在/var/www目录下。

**如无额外说明，本文中的相对路劲都是相对于/var/www目录的。**

```shell
mkdir /var/www

# extract the deployment package
unzip eos.zip -d /var/www

cd /var/www/eos

# init
chmod 755 eos-*
./eos-init

# install dependencies
play deps deploy/server

# remove the uncompatible jar file
rm deploy/server/lib/guice-4.0.jar
```

#### 配置

默认情况下服务器端使用:

* 基于本地文件存储的H2数据库。
* 使用本地文件存储安装的app。

可以根据需要修改'conf/custom.conf'以适应需求.

#### 运行

编辑脚本'eos-server', to modify the three properties:

```shell
# path to the executable file of Play Framework
PLAY=/opt/play/current/play

# path to the directory of eos
RUNDIR=/var/www/eos

# path to the pid file 
PIDFILE=/var/www/eos/deploy/server/server.pid
```

启动或停止:

```shell
# using the script file 'eos-server'
# start
./eos-server start
# stop
./eos-server stop

# or you can use the play command directly
# start
play start deploy/server
# stop
play start deploy/server
```

以特定环境名运行（比如这里使用dev）:
```shell
play start deploy/server --%dev
```





