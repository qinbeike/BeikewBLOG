第一章 Github基本使用方法
======================

1.1 基本操作
---------------------

提交本地项目到GitHub
1、 通过git shell进入项目文件夹，输入命令：git init 将项目文件夹变为本地git仓库；
2、 把项目文件夹中需要提交的文件添加到暂存区中，命令：git add .
3、 通过git commit -m "注释内容"把项目提交至仓库
4、 Github上设置ssh密钥后，新建远程仓库后，将通过命令： git remote add origin https://github.com/yourname/仓库名.git 将本地仓库与远程仓库关联
5、 通过git push -u origin master 将本地仓库项目提交至远程仓库
注： origin是远程仓库的别名，master为仓库的主干分支


1.2 分支操作
---------------------

显示分支： git branch
创建并切换分支：git checkout -b branchname 等同于 git branch branchname  git checkout branchname
合并分支： 分支A已创建完成，想要将分支A与master主干分支合并时，首先切换到master分支，然后git merge --no-ff A（--no-ff
是为了在历史记录中明确记录本次分支合并）

1.3 更改提交的操作
---------------------

git reset --hard：回溯历史版本