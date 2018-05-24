### git 
1. git 全局配置
    > git config --global user.name "Your Name"

    > git config --global user.email "email@example.com" 
    
2. git init
    > 把当前的目录变成git可以管理的仓库

3. 常用
    - git add
        + git add . 不包括被删除的文件
        + git add -u 仅监控已被add的文件
        + git add -A 上面两个功能的集合
    - git commit 
        + git commit -m '本次提交的说明'
    - git status
        + 查看仓库当前状态
    - git diff [name]
        + 查看差异
    - git log
        + 查看提交日志
        + git log --graph --pretty=oneline --abbrev-commit  查看分支合并情况
    - git reset
        +  git reset --hard [id] 回退到那个版本
    - git reflog
        + 记录你的每一次命令
    - git checkout 
        + git checkout -- file 丢弃工作区的修改
        + git checkout -b [分支名] 创建并切换到这个分支上
        + git checkout [分支名] 切换到这个分支上
    - git branch 
        + 查看当前分支
        + git branch [分支名] 创建这条分支
        + git branch -d [分支名] 删除这条分支
        + git branch -D [分支名] 强行删除没有被合并过的分支
        + git checkout -b [分支名] origin/[分支名] 在本地创建和远程分支对应的分支
        + git branch --set-upstream [分支名] origin/[分支名] 建立本地分支和远端分支的关联
    - git merge 
        + 命令用于合并指定分支到当前分支
        + git merge --no-ff -m 'docs' [分支名] 本次合并创建一个新的commit 不用 fast forward
    - git stash
        + 把当前的工作现场储存起来，等以后恢复在继续工作
        + git stash list 查看临时储存列表
        + git stash pop 恢复的同时把 stash 内容删除
    - git tag 
        + 打标签
        + 标签总和某个commit挂钩 如果这个commit出现在两个分支 那么这两个分支都可以看到这个标签
        + git tag <tagname> 新建一个标签
        + git tag -a <tagname> -m "blablabla..." 指定标签信息
        + git tag 查看所有标签
        + git tag -d <tagname> 删除本地标签
        + git push origin <tagname> 推送一个本地标签
        + git push origin --tags 推送全部未推送的本地标签
        + git push origin :refs/tags/<tagname> 删除远端一个标签
    - git push 
        + 把本地库所有内容推送到远程库上
    - git clone 
        + 克隆仓库到本地
    - git pull 
        + 拉取别人提交的代码
    - git remote
        + git remote -v 查看远程库信息
        + git remote add [name] xxx@xxx 关联远程库
        + 要关联两个远程库 设置不同的name
        + 推送的时候git push [name] master