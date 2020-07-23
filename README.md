（远程代码下载到本地新建分支；对比区别后在合并）
1. 查看远程仓库
  git remote -v
2. 从远程获取最新版本到本地temp分支上
  git fetch origin master:temp
3. 比较本地的仓库和远程参考的区别
  git diff temp
4. 合并temp分支到master分支
  git merge temp
5. 如果不想要temp分支了，可以删除此分支
  git branch -d temp
  如果该分支没有合并到主分支会报错，可以用以下命令强制删除git branch -D <分支名>


（本地新建分支完成开发；提交代码到远程git）
1. 查看当前分支，当前状态
  git branch
  git status
2. 创建并切换到分支
  git checkout -b [name]
3. 开发中~开发完成！
4. 提交修改到本地仓库
  git add .
5. 输入提交备注信息
  git commit -m "提交代码"
6. 提交修改到远程仓库
  git push origin [name]
7. 将项目切换到主分支master
  git checkout master
8. 合并代码
  git merge [name]
9. 提交修改到远程仓库
  git push origin master
