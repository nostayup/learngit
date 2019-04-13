# learngit

## 操作步骤
初始化文件夹：  
>git init

添加文件到缓存区：  
>git add filename

提交修改到工作区：  
>git commit -m "what you want to record"

显示工作区和缓存区的区别：  
>git diff

缓存区和版本库的区别：  
>git diff --cached

工作区和版本库里面的区别：  
>git diff HEAD -- file_name

查看当前状态：  
>git status

连接远程库：  
>git remote add origin  git@github.com:nostayup/XXXXXXX.git

如果远程库和本地库不一致，先让远程文件同步到本地，执行：  
>git pull --rebase origin master

把当前分支提交到远程库：  
>git push -u origin <branch_name>

## 版本退回或者前进  
显示从最近到最远的提交日志，准备穿梭回过去:  
>git log

退回过去的版本：  
>git reset --hard XXXX版本号XXX

记录每次的操作，前面有版本号，用于穿梭回未来：  
>git reflog

撤回最近一次工作区的修改,包括误删文件  
>git checkout -- file_name 

撤回暂存区的更改：  
>git reset HEAD file_name

从版本库里面删除文件，先从工作区删除文件，然后  
>git rm file_name;  
>git commit -m "what you want to say"

## 创建合并分支  
创建并指向新的分支,-b相当与git branch new + git checkout new,
以后的修改和提交都是在这个分支上了  
>git checkout -b new_branch  
查看当前分支：  
>git branch  
切换回master分支：  
>git checkout master  
把某分支合并到当前所在的分支：  
>git merge <name>  
删除旧的用过的分支：  
>git branch -d new_branch  








