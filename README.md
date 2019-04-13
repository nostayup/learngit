# learngit

操作步骤
==========
初始化文件夹：
git init

添加文件到缓存区：
git add filename

提交修改到工作区：
git commit -m "what you want to record"

显示工作区和缓存区的区别：
git diff

连接远程库：
git remote add origin  git@github.com:nostayup/XXXXXXX.git

如果远程库和本地库不一致，先让远程文件同步到本地，执行：
git pull --rebase origin master

提交到远程库：
git push -u origin master