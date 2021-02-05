# 基于Github、Typora的打卡流程

Github用于团队监督与交流，Typora用于编辑markdown文档

## Typora上手

1. Typora下载

   官网下载较慢，用这个链接https://gitee.com/typora-mirror/Typora-Mirror/releases 

   [国内Typora镜像]: https://gitee.com/typora-mirror/Typora-Mirror/releases

2. Typora使用方法

   Typora是一个优秀的Markdown文本编辑器，只需要学习Markdown基本语法即可。Markdown语法速览：https://www.jianshu.com/p/191d1e21f7ed

3. Typora的使用场景

   用于文件的编写，将文件存入本地文件夹，之后上传到Github团队工作区。文件模板：https://github.com/Programmers-With-Dreams/GithubTest/tree/dyd


## Github使用

### Git

官网下载，Next安装。

[Git30min入门]: https://www.runoob.com/git/git-tutorial.html

### Github建仓基本命令

首先在Github上建立一个仓库，然后建立本地仓库与远程仓库的链接

#### 本地仓库未建立的情况

新建文件夹，打开进入，右击Git Bash Here,命令行输入
git init 
git add README.md
git commit -m "first commit"
git branch -M **main**（分支名称）
git remote add **origin**（远程仓库别名） https://github.com/Programmers-With-Dreams/ee.git（远程仓库链接）

【

push之前需要将本地文件先add到暂存区，再commit到本地仓库

git add .

git commit -m "第x周提交"

】

git push -u **origin**（远程仓库别名） **main**（分支名称）



#### 已经存在本地仓库的情况

需要进行以下的操作

git remote add **origin**（远程仓库别名） https://github.com/Programmers-With-Dreams/ee.git（远程仓库链接）
git branch -M **main**（分支名称）

【

push之前需要将本地文件先add到暂存区，再commit到本地仓库

git add .

git commit -m "第x周提交"

】

git push -u **origin**（远程仓库别名） **main**（分支名称）

### Leetcode仓库建立

在本地使用Git init建立一个文件夹，使用Git remote add建立本地仓库与远程仓库https://github.com/Programmers-With-Dreams/Leetcoders.git的链接，使用git branch -M建立自己的分支（比如dyd，lsq，fqc）,在本地git add，git commit之后就可以使用git push -u 提交到远程仓库了。