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
    - git merge 
        + 命令用于合并指定分支到当前分支
    - git push 
        + 把本地库所有内容推送到远程库上
    - git clone 
        + 克隆仓库到本地