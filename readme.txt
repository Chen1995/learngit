哈哈 我改了这个 http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/0013743858312764dca7ad6d0754f76aa562e3789478044000



git 常用操作：
	创建版本库：
		mkdir learngit
	进入文件夹：
		cd learngit
	查看当前目录：
		pwd
	修改文件，将文件提交到版本库：
		git add 文件名
		git commit -m "日志"
	查看历史更改记录(如果输出内容太多可以加上“--pretty=oneline”，类似3628164...882e1e0一大串数字表示版本号)：
		git log
	回退到上一个版本（上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100）：
		git reset --hard HEAD^   或者git reset --hard 版本号（版本号的一部分）
	查看当前版本内容：
		cat 文件名

	连接远程仓库：
	    git remote add origin git@github.com:Chen1995/learngit.git（文件名）

	把本地库的所有内容推送到远程库上：
	    git push -u origin master
	    git push origin master


	从远程库克隆到本地库
		git clone git@github.com:Chen1995/gitkill.git
	
	创建分支，然后切换到dev分支（git checkout命令加上-b参数表示创建并切换，相当于以下两条命令：git branch dev     git checkout dev）
		git checkout -b dev

	查看当前分支（git branch命令会列出所有分支，当前分支前面会标一个*号）
		git branch
