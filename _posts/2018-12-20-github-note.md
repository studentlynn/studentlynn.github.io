---
layout: post
title: "「语法」10分钟掌握github"
subtitle: "Learning github in 10 min"
author: "Lynn"
header-img: "img/post-bg-halting.jpg"
header-mask: 0.3
tags:
  - 语法
  - 待续
---




$ give me super-powers


## 本文参考资料：
[简书 献给写作者的 Markdown 新手指南](https://www.jianshu.com/p/q81RER)

# GIt及gitbook基础入门 10-30

### git的原理
* 集中式版本控制：版本库是集中存放在中央服务器的，干活的时候，要先从中央服务器取得最新的版本，然后开始干活，干完活了，再把自己的活推送给中央服务器。中央服务器就好比是一个图书馆，你要改一本书，必须先从图书馆借出来，然后回到家自己改，改完了，再放回图书馆。

* 分布式版本控制系统：首先，分布式版本控制系统根本没有“中央服务器”，每个人的电脑上都是一个完整的版本库，这样，你工作的时候，就不需要联网了，因为版本库就在你自己的电脑上。既然每个人电脑上都有一个完整的版本库，那多个人如何协作呢？比方说你在自己电脑上改了文件A，你的同事也在他的电脑上改了文件A，这时，你们俩之间只需把各自的修改推送给对方，就可以互相看到对方的修改了。分布式版本控制系统通常也有一台充当“中央服务器”的电脑，但这个服务器的作用仅仅是用来方便“交换”大家的修改，没有它大家也一样干活，只是交换修改不方便而已。

### 绑定账号
```
git config --global user.name "Your Name" 
git config --global user.email "email@example.com" 
```
注意git config命令的--global参数，用了这个参数，表示你这台机器上所有的Git仓库都会使用这个配置，当然也可以对某个仓库指定不同的用户名和Email地址

### 仓库等关系
* repository：版本库，又叫做仓库
* 缓冲区的概念：git status 查看仓库的状态；文件做修改后，用add分次提交文件，然后一个commit提交后，文件才会做出修改并提交！~注意，一定要commit，不然多次 add 文件可能还是没有更改，会出错的！
```bash
$ mkdir learngit
$ cd learngit
$ pwd
```

* git init：将本目录设置为git管理的仓库
* **git add readme.txt** 添加文件到仓库
* **git commit** 提交
```
git init
git add readme.txt
git commit -m "wrote a readme file"

```
* 【注意】编辑txt的话，不要用windows自带的记事本。Notepad++的默认编码设置为UTF-8 without BOM


* **git status** 仓库当前的状态
* **git diff** 如果status显示有变化，则查看不同版本文件的差别
* **git log** 提交文件的历史
* **git log --pretty=oneline** 提交文件的历史，只看关键的**版本号**（一串乱码的那种）
* **git reset --hard 1094a** 版本回退，其中1094a是log里面看到版本号的前面几位，不用写全，能识别出来就行~~
* **git reflog** 查看每一次回退的内容~~

* **cat readme.txt** 查看文件内容~~



## gitbook的原理











## 本文参考资料：
[廖雪峰的官网](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)

