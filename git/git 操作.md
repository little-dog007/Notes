[git删除未跟踪文件]()  
[git创建本地分支与远程分支]()
[当前分支rebase某个远端分支]()
[回退]()



- 删除未跟踪文件：git clean -f

- git创建本地分支与远程分支:（__不需要到github上手动创建，比较麻烦__） 
   1.  git branch 分支名（__注意是基于当前分支__）
  2.   git checkout 分支名
  3.   git push （__根据提示敲命令，此时会在远端自动创建分支并跟你的分支关联__）

- 当前分支rebase某个远端分支:  
git pull origin master --rebase

- 回退有两种方式：
    1. git reset commit-号  ： 这个需要手动回滚
    2. git reset --hard commit-号 : 不需要手动回滚

