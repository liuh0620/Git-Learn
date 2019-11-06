# Git命令的使用

## Git命令使用
1. Git配置类命令：
    - 配置git的用户名：  
    `git config --global user.name "liuh"`

    - 配置git的邮箱：  
    `git config --global user.name "872266255@qq.com" `

    - 查看git的配置信息：  
    `git config --list `

    - 查看git的版本信息  
    `git --version `

----
 2. 新建代码仓库类命令：   
     - 在当前目录新建一个Git代码库：   
     `git init`

     - 下载一个项目和它的整个代码历史：    
     url格式：https://github.com/[username]/reposName   
     `git clone [url]`
---

  3. 添加、删除和命名文件命令：
      - 添加指定文件到暂存区：    
      `git add [file1] [file2]`

      - 删除工作区的文件，并且将这次删除放入暂存区：   
      `git rm [file1] [file2]`

      - 修改文件名，并且将这个改名放入暂存区   
      `git mv [file-origin] [file-renamed]`

----
 4. 代码提交命令：  
     - 提交暂存区到仓库   
     `git commit -m [message]`   

     - 直接从工作区提交到仓库（前提是该文件已经有仓库中的历史版本）  
     `git commit -a -m [message]`

----
 5. 查看仓库的状态：  
    - 查看变更信息：  
    `git status`  

    - 显示当前分支的历史版本：   
    `git log`  
    `git log --oneline`  

    - 查看具体版本的修改：  
    `git show [哈希值]`

---
 6. 同步到远程仓库：  
     - 增加远程仓库，并命名：   
     `git remote add [shortname] [url]`   
     如：`git remote origin https://github.com/liuh0620/demo`  
     附：origin:表示给URL命的名字，origin就代表URL的地址。

     - 查看当前仓库是否跟远程仓库有建立联系命令：  
     `git remote -v`  

     - 将本地的提交推送到远程仓库   
     `git push [remote] [branch]`  
     如：`git push origin master`  
     此命令代表将本地master分支推送到远程的仓库origin上。

     - 将远程仓库的提交下拉到本地仓库   
     `git pull [remote] [branch]`
