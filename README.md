# git_command_learn
git命令操作学习

git init                  初始化

git branch            查看所有的分支

git branch -d <BranchName>	        删除本地仓库分支

git push origin --delete <BranchName>       删除远程仓库分支

git status                		工作区文件状态

git add                   		将工作区文件提交到暂存区

git commit -m ""          	将暂存区文件，提交到本地仓库，并添加注释

git reset HEAD -- <file>  	拉取最近一次提交到版本库的文件到暂存区，该操作不影响工作区      
  
git checkout -- <file>    	拉去暂存区文件，并将其替换成工作区文件

git pull origin master      	拉去远程仓库的master分支并与本地仓库代码合并（fetch+merge）

git push -u origin master	将本地仓库中的代码推送到远程仓库的master分支上

git fetch origin/master temp	     拉去远程仓库的master分支代码到本地仓库并新建分支temp

git diff temp		比较本地的master分支代码与temp分支代码的区别

git tag -a V0.1.3 -m 	“注释″     -a 后面跟着的是版本号，-m后面是注释。打tag是在代码commit到本地仓库后。

git push origin --tags 	提交所有tag至服务器端，普通的git push origin master是不会提交tag的。

git tag --list  		 查看已有tag列表

git checkout [tag/branch/commit]  	切换到指定tag/branch/commit都是此命令

git tag -d V0.1.3			删除标签

git push origin :refs/tags/0.1.3	删除远程仓库里的tag