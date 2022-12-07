该项目是为了方便在对CMS漏洞进行复现的时候花费大量的时间在网上搜索漏洞源码，从而有了此项目。此项目仅为安全研究使用并且所有CMS存在大量漏洞，请勿以此建站。

## 环境搭建

经过测试，本项目的源码均可使用docker安装运行

```
# 拉取镜像
docker pull medicean/vulapps:base_lamp
# 利用镜像启动容器
docker run -d -p 8080:80 medicean/vulapps:base_lamp
```

镜像信息

```
系统版本：Ubuntu 14.04.5
Apache版本：2.4.7
PHP版本：5.5.9
MySQL版本：5.5.61
Web路径：/var/www/html
数据库账号密码：root/root
```

部分CMS需要php-curl扩展，进入到容器里执行

```
apt-get update
apt install php5-curl
```

然后重启apache或者docker即可。
