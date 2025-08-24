**git init**
**git remote -v**
**git remote add xx https://**
**git remote -v**
**git checkout master**
**git add .**
**git commit -m" "**
**git push xx master**

### （一）
#### 1. git checkout -- \<filename>
>本地仓库代码改动-->退回远程仓库之前的文件
#### 2. git reset HEAD \<filename>
>把add暂存区的内容舍弃，回退到工作区状态(文件名可加可不加)
#### 3. git reset --hard `<commit的四位>`
>找回的话使用**git reflog`(查看head改动日志)`**,然后在**git reset --hard \<commit>**

![命令图片](/pictures/1.png)

#### 4. git diff HEAD -- \<filename> 
>查看远程仓库跟本地仓库修改文件的区别

### （二. 分支）
#### git branch 
>看本地分支
#### git branch -r:
>看远程跟踪分支。
#### git branch -a:
>看所有（本地和远程跟踪）分支。
#### git branch -vv
> 看本地分支的详细信息（最新提交、上游分支、同步状态）。
#### git checkout -b <branchname>
>创建并切换分支
#### git checkout <branchname>
>切换分支
#### git branch -d <branchname>
>删除分支
#### git push origin <filename>:main
>指定本地分支推送到远程仓库