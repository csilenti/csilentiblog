---
title: Linux系统命令
date: 2024/3/26 1:13:00
updated:
cover:
categories:
tags:
---

## 通过 CMD 连接到远程的 Linux 系统

- 在 Windows 系统上按 `win` + `R` ，然后在弹出的 `运行` 窗口中输入 `cmd` ，打开默认的终端程序。

- 执行以下命令发起ssh连接，进入Linux系统。

~~~shell
ssh <user>@<host>
# user 是 xxx
# host 是 xxx
# 示例： ssh root@10.10.10.10
~~~



##### 切换目录(cd)

~~~~
cd /              切换到根目录
cd /bin           切换到bin目录
cd ../            切换到上一级目录
cd ~              切换到home目录
cd -              切换到上次访问的目录
cd xx(文件夹名)    切换到本目录下的名为xx的文件目录，如果目录不存在报错
cd /xxx/xx/x      可以输入完整的路径，直接切换到目标目录，输入过程中可以使用tab键快速补全
~~~~



##### 查看目录(ls)

~~~
  ls                查看当前目录下的所有目录和文件
  ls -a             查看当前目录下的所有目录和文件（包括隐藏的文件）
  ls -l             列表查看当前目录下的所有目录和文件（列表查看，显示更多信息），与命令"ll"效果一样
  ls /bin           查看指定目录下的所有目录和文件 
~~~



##### 创建目录(mkdir)

~~~
mkdir tools         在当前目录下创建一个名为tools的目录
mkdir /bin/tools    在指定目录下创建一个名为tools的目录
~~~
