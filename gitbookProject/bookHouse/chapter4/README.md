# git


## git常用命令:
- 初始化本地仓库
```
git init
```
- 查看服务器分支和本地分支，标记*的表示当前所在的分支
```
git branch -a
```
- 将工作区的代码提交到暂存区
```
git add .
```
- 将暂存区的代码提交到本地仓库区(提交后,暂存区的内容就清空了)
```
git commit -m "注释部分"
```
- 把远程dev分支上的内容拉下来
```
git pull origin dev
```
- 把当前分支上的内容推送到远程服务器的dev分支
```
git push origin dev
```

- 把服务器上的dev分支和master合并的步骤:
1. 假如本地当前默认的是dev分支
2. 做完文件编辑的动作
3. git merge master     --> 让当前的本地的(dev和master分支进行合并)
4. git push origin master   --> 把最新的内容推送到服务器的master分支

- 把本地的rsa_dev_rc分支推送到远程仓库
```
git push origin HEAD:rsa_dev_rc
```

- 把本地的rsa_dev_rc分支推送到远程仓库(远程有这个仓库就覆盖,没有会自动创建)
```
git push origin HEAD:rsa_dev_rc
```