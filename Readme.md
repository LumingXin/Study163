git常用命令：</br>
四种状态</br>
    1.Untracked 未被追踪</br>
    2.Modified 已修改的</br>
    3.Staged 已暂存的</br>
    4.Committed 已提交的

三层结构</br>
    1.working-directory 工作区 git dd</br>
    2.staging-index 暂存区 git commit -m 'XXX'</br>
    3.git-directory 版本库 git push

git config</br>
    git config --global user.name xxx</br>
    git config --global user.email xxx@x.xx
    
git@github.com:youname/项目名称.git

git config --global user.name "xxx"</br>
git config --global user.email "xxx@xxx.com"</br>
$ ssh-keygen -t rsa -C youremail@example.com</br>
[c 盘->用户->自己的用户名->.ssh]

git remote -v 查看远程仓库

git add 将文件保存到暂存区
git commit -m 'XXX' XXX表示提交说明，该命令是将文件从暂存区提交到提交区
git commit -am 'XXX' 等同于git commit -a -m 'XXX'  XXX表示提交说明，该命令是将文件直接提交到提交区，仅对已经有过提交记录的文件有效，新创建的文件依旧需要git add后再git commit
git push 提交内容到远程仓库

git reset HEAD filename 拉取最近一次"提交区"文件到"暂存区"但不影响"工作区"
git checkout -- filename 拉取"暂存区"文件替换到"工作区"

git rm --cahead filename 删除暂存区的文件
git rm -f filename 删除暂存区和工作区的文件（无视修改）

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