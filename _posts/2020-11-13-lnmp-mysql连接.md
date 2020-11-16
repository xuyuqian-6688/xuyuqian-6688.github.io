---
layout: page

title: "LNMP环境搭建mysql连接问题"

subtitle: "运维小菜鸟"

date:  2020-11-13 15:21:22 +0530

categories: ["专业"]
---

# 本地连接服务器mysql出错问题



## navicat连接

~~~ 
使用常规连接不要使用SSH通道连接
~~~

## 服务器mysql修改配置文件

~~~
地址：vim /etc/mysql/mysql.conf.d/mysqld.cnf
1、注释掉配置#bind-address           = 127.0.0.1
2、pork=3306
~~~

~~~ 
连接mysql
进入mysql库 修改user表root字段Host字段，把host字段值改为%
保存重启
查看端口 netstat -an|grep 3306  
	tcp6       0      0 :::3306                 :::*                    LISTEN     
    tcp6       0      0 172.27.30.52:3306       121.32.88.197:60364     ESTABLISHED
    tcp6       0      0 172.27.30.52:3306       121.32.88.197:10816     ESTABLISHED

~~~

## laravel同理

- 修改env文件，配置mysql以后可以正常访问