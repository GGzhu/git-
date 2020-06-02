git官方教程
https://git-scm.com/book/zh/v2

1-设置用户名
git config --global user.name 'GGzhu'

2-设置用户邮箱
git config --global user.email '111@qq.com'

3-同步远程仓库
git pull

具体教程：
https://www.cnblogs.com/sgdd123/p/8338403.html

修改默认用户密码：
vi .git/config
url=https://用户名:密码@github.com/用户名/仓库名.git

三步曲:

1.克隆远程仓库到本地: git clone 仓库地址
2.提交文件到暂存区: git add 文件
3.查看当前文件状态: git status 查看状态
4.提交文件到本地仓库: git commit -m "描述"
5.同步本地与远程仓库: git push 

总结：
Git基本常用命令如下：
创建目录mkdir
显示当前目录的路径：pwd
把当前的目录变成可以管理的Git仓库：git init
把xx文件添加到暂存区：git add xx
提交文件：git commit -m "注释"
查看仓库状态git status
查看xx文件修改了哪些内容git diff xx
查看历史记录git log
回退版本git reset --hard HEAD^或者git reset --hard HEAD~50
查看文件cat xx
查看历史记录的版本号idgit reflog
把xx文件在工作区的修改全部撤销git checkout -- xx
删除xx文件rm xx
关联一个远程库git remote add origin 地址
把当前master分支推送到远程库git push -u(第一次要用-u 以后不需要) origin master
从远程库中克隆https://github.com/duanmingpy/remote_repo.git
创建dy分支并切换到git checkout –b dy
查看当前所有分支git branch
切换回master分支git checkout master
在当前的分支上合并dy分支git merge dy
删除dy分支git branch –d dy
创建分支git branch name
把当前的工作隐藏起来，等以后恢复现场后继续工作git stash
查看所有被隐藏的文件列表git stash list
恢复被隐藏的文件，但是内容不删除git stash apply
删除文件git stash drop
恢复文件的同时删除文件git stash drop
查看远程库的信息git remote
查看远程库的详细信息git remote -v
把master分支推送到远程库对应的远程分支上git push origin master
