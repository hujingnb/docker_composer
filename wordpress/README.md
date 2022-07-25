## 使用步骤

1. 复制`.env.example`文件为`.env`并重写其中的变量
2. 启动`docker-compose up`
3. 访问本地80端口即可

## 其他内容

**指定域名**

若需要为`wordpress`指定域名, 修改`nginx/conf/default.conf`文件即可.

**后台限定 IP 访问**

修改`nginx/conf/default.conf`文件, 将其中的访问限制打开即可. 

**mysql5.7版本**

因为使用`docker`的目的, 是为了方便后面迁移项目. 我在使用8.0的情况下, 无法通过直接复制共享目录的方式重启, 故切换版本到5.7 . 

原因如下: `https://stackoverflow.com/questions/64146845/mysql-not-starting-in-a-docker-container-on-macos-after-docker-update`. 

可根据需要修改版本

**https**

如果需要开启 https 服务, 请使用`nginx/conf/default.conf.https`文件, 并修改其中关于域名和证书的部分. 证书请自行解决. 

