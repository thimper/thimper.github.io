---
title: Mac PHP安装
date: 2019-02-21 21:26:01
tags: php
---

# Apache 启动

- 启动/关闭 apache 服务
  ` sudo apachectl start/stop/restart`
- 查看 apache 版本
   `sudo apachectl -v `
-  apache 安装路径
    > /private/etc/apache2
- apache 配置文件
    > /private/etc/apache2/httpd.conf
- apache 服务部署目录
    > /资源库/WebServer/Documents/

# PHP 配置

- apache 添加 php模块支持
   修改配置 `/private/etc/apache2/httpd.conf`
   找到配置
   `#LoadModule php5_module libexec/apache2/libphp5.so`
   将前方的#删除