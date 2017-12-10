# git


## git常用命令:
git init       --> 初始化<br/>
git branch -a  --> 查看服务器分支和本地分支，标记*的表示当前所在的分支<br/>
git add .<br/>
git commit -m "注释部分"<br/>
git pull origin dev  --> 把远程dev分支上的内容拉下来<br/>
git push origin dev  --> 把当前分支上的内容推送到远程服务器的dev分支<br/>


把服务器上的dev分支和master合并的步骤:
1. 假如本地当前默认的是dev分支
2. 做完文件编辑的动作
3. git merge master     --> 让当前的本地的(dev和master分支进行合并)
4. git push origin master   --> 把最新的内容推送到服务器的master分支


将服务器上的分支内容撤销到以前的某个版本的步骤:
git log      --> 找打commit 的ID号
git reset --hard <commit_id>