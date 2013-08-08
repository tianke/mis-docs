title: 项目工场开发工程师 - System - Max OS X
date: 2013-06-18 11:39:31
tags: Mac Terminal homebrew
---

# MacOS x

## Terminal 终端

### 打开目录

    $ cd ~          # 打开当前用户的根目录
    $ cd /          # 打开根目录
    $ cd /usr/      # 打开绝对目录
    $ cd user/      # 打开相对目录
    $ cd ..         # 打开上级目录
    $ open .        # 将当前目录在Mac的Finder里显示

### 列出所有文件

    $ ls            # 列出所有文件
    $ ls -a         # 列出所有文件包括隐藏文件
    $ ls -G         # 列出所有文件，并根据文件的特性显示不同的颜色

### 创建

    $ touch index.html      # 创建一个新的文件

### 删除

    $ rm index.html         # 删除一个文件，但无法删除文件夹
    $ rm -rf index          # 强制并且遍历删除所有的index文件夹及文件夹内文件
                            # -r 表示 遍历 -f 表示强制

### 移动/重命名

    $ mv index.html index2.html         # 将index.html改名为index2.html
    $ mv first/index.html second/       # 将first内的index.html移动到second

### 复制

    $ cp index.html.example index.html

### 替身（快捷方式）

    $ ln -s index.html /usr/local/bin/index.html

### 解压缩

    $ tar -zxvf index.tar

### 管理员权限打开

    $ sudo mv index.html index2.html

### 设置文件和文件夹权限

    $ chmod -R 777 index

## vim

当没有可视化界面时，我们要在Terminal中编辑一个文件，就需要使用到vim

### 打开文件

    $ vim index.html

其他更多资料参考：https://zh.wikipedia.org/wiki/Vim

## HomeBrew

### 简介

我们经常需要安装大量相关的软件来作为我们的工具，或者是运行我们的某些代码，比如我们需要安装 git 来管理我们的代码版本，需要安装 redis 或者 mysql 之类的程序。

在windows里，通常我们会打开一个已经被编译好的exe文件执行。

在 *nix 里，我们可以选择原生编译的方式来安装程序，比如 make 命令，但是这是非常辛苦的事情，因为没有整理好相关的依赖文件和路径配置，往往会满头大汗，痛不欲生。

而这个时候我们需要用更简单的方式，那就是软件包管理工具，就如同 linux 上的 apt 和 yum一般。

*先前往官网进行了解和对比，以防介绍网站里的资料过旧*
Homebrew 官网：http://mxcl.github.io/homebrew/index_zh-cn.html
相关介绍和使用文件：http://linfan.info/blog/2012/02/25/homebrew-installation-and-usage/

### 常用功能的概念理解

软件包管理工具最常做的几个事情：

1. 搜索软件包
2. 安装软件包
3. 移除软件包
4. 更新软件包

### 神奇的中国，神奇的墙

由于我们身在神奇的中国，有一堵神奇的墙，他的名字作为 GFW (中国国家防火墙)，他神奇地封锁了 http://code.google.com ，注意是http协议，所以，是的，我们可以通过https协议访问到它，https://code.google.com。

具体解决办法参考：http://leegorous.net/blog/2012/08/10/how-to-skip-download-in-brew-install/
