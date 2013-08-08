title: 项目工场开发工程师 - Tools - git
date: 2013-06-18 11:39:35
tags:
---

# git

## 简介

分布式代码版本控制工具，团队协作，开源开发等特点，同时适合小规格和超大规模的项目开发，比如linux内核的开发，就是有全球开源贡献者同时参与。

## Mac 上 安装 git

    $ brew install git

## ubuntu 上 安装 git

    $ apt-get install git

## GUI（可视化界面）版 git 管理工具

1. SourceTree for mac, windows
2. Github for mac, windows

在开发环境里建议使用GUI工具，提高工作效率；
在部署环境下，通常服务器只有终端，故建议使用命令行的方式。

## 基本概念

    $ git status
    $ git add
    $ git remove
    $ git commit
    $ git trash
    $ git push
    $ git pull
    $ git remote
    $ git branch
    $ git tag
    $ git merge

## 学会使用git

参考书籍：《pro git》http://ishare.iask.sina.com.cn/f/16096245.html
*必须花些时间读完该书，充分理解git的分支概念及操作*

## 将代码存放在第三方网站

### github
*你学习编程和逐步融入国际程序界的最佳途径*
https://github.com

百科介绍（由于wikipedia被无良的祖国贪官墙掉了，所以只能看百度百科了）：
http://baike.baidu.cn/view/3366456.htm

如何高效利用github
http://www.yangzhiping.com/tech/github.html

### bitbucket
*因为github上托管的项目都是公开的，所以我们要存放私有项目，就得用bitbucket了*

bitbucket本身也做得很棒，但是由于公司较小，国内没有服务器加速访问，再加上中国贪官不定时墙掉托管bitbucket的亚马逊EC2云主机，所以push和pull项目的时候比较蛋疼。

https://bitbucket.org

### gitcafe
*最后我们有想要托管私有项目，又不想被贪官挡在墙外该怎么办呢？那就是 gitcafe*

https://gitcafe.com
