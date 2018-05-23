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
    