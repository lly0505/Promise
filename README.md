# Promise
# git 更新远程代码到本地仓库
`（远程代码下载到本地新建分支；对比区别后在合并）`
    1. 查看远程仓库
        git remote -v
    2. 从远程获取最新版本到本地
        git fetch origin master:temp
    3. 比较本地的仓库和远程参考的区别
        git diff temp
    4. 合并temp分支到master分支
        git merge temp
    5. 如果不想要temp分支了，可以删除此分支
        git branch -d temp
    如果该分支没有合并到主分支会报错，可以用以下命令强制删除git branch -D <分支名>
` git拉取代码到本地 `
    1. git config --global user.name "git权限的名称"
    2. git config --global user.email "git的帐号"
    提交本地代码到远程服务器

    第一步：git pull 先获取代码

    第二步：git status 查看状态

    第三步：git add 添加要提交的代码地址

    第四步：git commit -m "备注提交代码的功能"

    第五步：git push 提交代码到远程服务器
