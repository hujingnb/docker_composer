# 介绍

通过`docker`创建PHP开发环境. 

# 使用说明

1. 将项目`clone`到你本地的任意位置
2. 修改根目录下的 `.env` 文件, 将其中的工作目录修改为自己适合的
4. 将 `config/nginx/config/default.conf/default.conf` 文件中的项目路径修改为你自己的项目路径
4. 执行命令: `docker-compose up`
5. 访问 `localhost` 测试

完成. 修改了其中的两个内容, 然后即可一键启动. 

可正常创建多个域名映射关系. 

---

当然, 整个`docker-compse`是一个系统, 你可以在其中添加你需要的docker镜像, 

