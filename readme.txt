git常用命令：

git add 将文件保存到暂存区
git commit -m 'XXX' XXX表示提交说明，该命令是将文件从暂存区提交到提交区

git reset HEAD filename 拉取最近一次"提交区"文件到"暂存区"但不影响"工作区"
git checkout -- filename 拉取"暂存区"文件替换到"工作区"

git rm --cahead filename 删除暂存区的文件
git rm -f filename 删除暂存区和工作区的文件（无视修改）

git diff 比较工作区和暂存区的差异
git diff --staged 比较暂存区和版本库的差异



VsCode
Shitt+Art+↓ //复制当前行
Shift+Ctrl+K //删除当前行
Ctrl+Enter //新起一行