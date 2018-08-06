git常用命令：

git config --global user.name "xxx"
git config --global user.email "xxx@xxx.com"
$ ssh-keygen -t rsa -C youremail@example.com
[c 盘->用户->自己的用户名->.ssh]

git remote -v 查看远程仓库

git reset HEAD filename 拉取最近一次"提交区"文件到"暂存区"但不影响"工作区"</br>
git checkout -- filename 拉取"暂存区"文件替换到"工作区"

git rm --cahead filename 删除暂存区的文件</br>
git rm -f filename 删除暂存区和工作区的文件（无视修改）

git diff 比较工作区和暂存区的差异</br>
git diff --staged 比较暂存区和版本库的差异</br>
git diff SHA1 SHA1 比较不同版本库的差异</br>
git diff brancgname 比较不同分支的差异

git stash 保存当前工作状态并返回修改之前的状态</br>
git stash list 查看保存的工作状态</br>
git stash apply stash@{number} 拉回保存的修改到本地</br>
git stash pop stash@{number}拉回修改 并删除记录</br>
git stash drop stash@{number} 删除保存的记录

VsCode
Shitt+Art+↓ //复制当前行</br>
Shift+Ctrl+K //删除当前行</br>
Ctrl+Enter //新起一行

