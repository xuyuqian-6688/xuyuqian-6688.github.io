---
layout: page
title: "搭建个人博客"
subtitle: "搭建github个人博客"
date:   2020-09-13 15:21:21 +0530
categories: ["web基础"]
author: "乾哥哥"
meta: "Springfield"
---

# 搭建个人技术博客

> 使用GitHub Pages + Jekyll 快速部署个人博客
>
> - GitHub Pages 
>
>   - 定义：GitHub网站给所有的用户提供了个人主页
>
>   - 如何访问：用户名.github.io
>   - 如何编写主页：建立一个用个人域名为项目名的远程版本仓库，只需要向该远程版本仓库中的master分支提交代码即可（该代码中必须要有个index.html文件）
>
> - Jekyll
>   - 定义：可以将markdown语法自动编译成html语法的一个工具
>   - 安装：不需要自己安装，在github网站当中预安装了
>   - 使用：不用人为使用，当请求个人域名的使用，GitHub服务器会自动读取仓库（以个人域名命名的那个远程版本仓库）中master分支中的代码，如果该代码为markdown语法，会自动调用Jekyll，将其编译为html，并返回客户端

- 建一个以个人域名为项目名的远程版本仓库
- 访问一个网站：主题网址：http://jekyllthemes.org/选择一个主题将其代码复制到我们仓库中的master分支
- （以上两部可以合并为一部，在主题仓库中点击fork，点击setting设置仓库名即可）
- 将远程版库中的代码克隆到本地
  - 复制仓库连接
  - 在文件夹中打开 git 执行克隆操作   git clone -b master 链接 目标文件夹
  - 从远程版本仓库克隆下来的代码会自动创建本地版本仓库
- 修改配置文件以及页面的内容
- 书写博客 blog

