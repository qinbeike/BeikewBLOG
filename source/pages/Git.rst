第一章 Github基本使用方法
======================

1.1 提交项目到Github
---------------------

#. 通过git shell进入项目文件夹，输入命令：git init将项目文件夹变为本地git仓库；

#. 把项目文件夹中需要提交的文件添加到暂存区中，命令：**git add .**

#. 通过**git commit -m** **"注释内容"**把项目提交至仓库

#. Github上设置ssh密钥后，新建远程仓库后，将通过命令： **git remote add origin https://github.com/yourname/仓库名.git** 将本地仓库与远程仓库关联

#. 通过 **git push -u origin master**将本地仓库项目提交至远程仓库

#. 注： origin是远程仓库的别名，master为仓库的主干分支::

    git init
    git add .
    git commit -m "first commit"
    git remote add origin https://github.com/yourname/仓库名.git
    git push -u orinin master



1.2 分支操作
---------------------

#. **显示分支**： **git branch**

#. **创建并切换分支**：**git checkout -b branchname**等同于 **git branch branchname**加上**git checkout branchname**

#. **合并分支**： 分支A已创建完成，想要将分支A与master主干分支合并时，首先切换到master分支，然后git merge --no-ff A（--no-ff是为了在历史记录中明确记录本次分支合并）

1.3 更改提交的操作
---------------------

#. **git reset --hard**：回溯历史版本

1.4 git clone
---------------------

从克隆远程仓库到本地时需要用git clone命令，git clone支持多种协议，HTTP、SSH、Git等等

#. git clone 远程仓库网址           #该命令在本地生成一个同名目录
#. git clone 远程仓库网址 本地库名称 #将远程仓库克隆到本地某个特定目录


1.5 git pull
---------------------

git pull的作用是获取某个远程分支并与本地分支合并，其完整命令格式为：

git pull 远程主机名 远程分支名：本地分支名




1.6 git remote
---------------------

git中每个远程主机必须指定一个主机名，git remote命令用于主机名的管理，常用命令如下

#. git remote #查看所有远程主机

#. git remote -v #同时查看远程主机的网址

#. git remote add 主机名 网址 #用于添加远程主机

#. git remote rm 主机名 # 用于删除远程主机

#. git remote rename 原主机名 新主机名 #用于远程主机改名


