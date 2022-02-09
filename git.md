  --慕课网 五月的夏天

https://www.imooc.com/video/22461

##### 1.仓库 <管理项目的中心>

项目代码的管理、项目进度的管理、开源

##### 2.上传代码到github

git init 初始化仓库

git add .   提交内容到暂存区

git commit -m "first commit"  对当前提交进行注释

git remote add origin git@github.com:xj17/mygitbook.git  推送到远程仓库

git push -u origin master 推送到master分支

##### 3.常用命令

git status 查看当前项目状态

git log 查看之前提交记录

git --version 检测当前git版本

git checkout --'文件名'  还原文件

git push origin master 修改内容后推送到远程仓库

##### 4.配置git的用户名和邮箱

git config --global user.name 'xj17'

git config --global user.email '1208845083@qq.com'

检查用户名和邮箱是否配置成功

git config --global --list

##### 5.关于.gitignore

上传github需要忽略的文件

##### 6.查看文件前后的变化

git log --pretty=online '文件名'









