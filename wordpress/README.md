## 使用步骤

1. 复制`.env.example`文件为`.env`并重写其中的变量
2. 启动`docker-compose up`
3. 访问本地80端口即可

## 其他内容

**指定域名**

若需要为`wordpress`指定域名, 修改`nginx/conf/default.conf`文件即可.

**mysql5.7版本**

因为使用`docker`的目的, 是为了方便后面迁移项目. 我在使用8.0的情况下, 无法通过直接复制共享目录的方式重启, 故切换版本到5.7 . 