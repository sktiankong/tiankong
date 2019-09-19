
先做自我介绍

第一堂课的要求：
	1.迟到、请假、课堂纪律（睡觉、戴耳机、玩游戏）。
	2.完成每日作业，整理笔记，每天要手写代码，一定要多敲。
	3.做好复习和预习
	
常用开发工具介绍：

    windows调用命名行:win+r  输入cmd 
    
    windows命令行怎么查看ip地址：
    	1.使用组合键win+r调出运行，输入CMD回车，进入命令提示符。
    	2.在命令提示符下输入 ipconfig/all。
    	IPV4地址就是本机的IP地址
    	
    mac如何查看ip地址：
    	1.ifconfig
    	2 inet 172.16.8.7 netmask
    	
    mac地址： ether 00:0e:c6:df:9c:3a


	1、 HBuilder 最常用快捷键
	
	    windows系统：
		
		Ctrl + d 删除本行
		Ctrl + Shift + R 复制上一行
		Ctrl + /  注释代码块
		Ctrl + Shift + /    开启关闭注释已选内容
		Ctrl+↑或↓ 移动当前行向上向下
		Ctrl + L 选中当前行
		
		mac：
		
		Command + d 删除本行
		Command + Shift + R 复制上一行
		Command + /  注释代码块
		Ctrl + Command+↑ 或 ↓ 移动当前行向上向下
		
	2.  webstorm
	3.  sublime
	4.  Editplus
	5.  ultraEdit
	6.  visual studio code
	7.  dreamweaver


第1单元  Ps及git

	1.1 Ps基本操作
		1.1.1 ps图层（5分）
		1.1.2 Ps测量（10分）
		
	1.2 Ps切图
		1.2.1 切图导出（10分）
		1.2.2 切图格式及质量（10分）


​	
	了解：
	
	Git 是一个开源的分布式版本控制系统，用于敏捷高效地处理任何或小或大的项目。
	Git 是 Linus Torvalds 为了帮助管理 Linux 内核开发而开发的一个开放源码的版本控制软件。
	Git 与常用的版本控制工具 CVS, Subversion 等不同，它采用了分布式版本库的方式，不必服务器端软件支持。
	
	Git 与 SVN 区别点：
	
	1、Git 是分布式的，SVN 不是：这是 Git 和其它非分布式的版本控制系统，例如 SVN，CVS 等，最核心的区别。
	
	2、Git 把内容按元数据方式存储，而 SVN 是按文件：所有的资源控制系统都是把文件的元信息隐藏在一个类似 .svn、.cvs 等的文件夹里。
	
	3、Git 分支和 SVN 的分支不同：分支在 SVN 中一点都不特别，其实它就是版本库中的另外一个目录。
	
	4、Git 没有一个全局的版本号，而 SVN 有：目前为止这是跟 SVN 相比 Git 缺少的最大的一个特征。
	
	5、Git 的内容完整性要优于 SVN：Git 的内容存储使用的是 SHA-1 哈希算法。这能确保代码内容的完整性，确保在遇到磁盘故障和网络问题时降低对版本库的破坏。


​		
	1.3 安装git
	
	1.3.1 安装git软件（15分）
	
	windows:
	
	下载地址：https://git-scm.com/download/win
	安装完成后，在开始菜单里找到“Git”->“Git Bash”，蹦出一个类似命令行窗口的东西，就说明Git安装成功！
	
	mac安装git
	
	安装homebrew，然后通过homebrew安装Git，具体方法请参考homebrew的文档：http://brew.sh/。
	/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	brew install git
	
	1.4 注册github, 码云（15分）
	
	GitHub:既可以让别人参与你的开源项目，也可以参与别人的开源项目。
	在GitHub上，可以任意Fork开源仓库；
	
	自己拥有Fork后的仓库的读写权限；
	
	可以推送pull request给官方仓库来贡献代码
	
	注册地址：
		https://github.com/join?source=login
	码云：
		https://gitee.com
		https://gitee.com/signup


​	
	1.5 使用git与github,管理项目（15分）
	
	推荐学习git网站 廖雪峰的官方网站: 
	https://www.liaoxuefeng.com/wiki/896043488029600

​	
​	
		1. 	git config --global user.name "wuhaijun"
			git config --global user.email 743532194@qq.com
		2.	查看已有的配置信息 git config --list

​			ssh-keygen -t rsa -C "youremail@example.com"  创建SSH Key		
			ssh -T git@github.com
			
			HTTPS：不管是谁，拿到url随便clone，但是在push的时候需要验证用户名和密码；
			SSH：clone的项目你必须是拥有者或者管理员，而且需要在clone前添加SSH Key。
				SSH 在push的时候，是不需要输入用户名的，如果配置SSH key的时候设置了密码，
				则需要输入密码的，否则直接是不需要输入密码的。
			
			
		git 工作流程：
		
		一般工作流程如下：
		
			克隆 Git 资源作为工作目录。
			在克隆的资源上添加或修改文件。
			如果其他人修改了，你可以更新资源。
			在提交前查看修改。
			提交修改。
			在修改完成后，如果发现错误，可以撤回提交并再次修改并提交。
			
		理解 工作区，暂存区，版本库	
		工作区：就是你在电脑里能看到的目录。
		暂存区：英文叫stage, 或index。一般存放在 ".git目录下" 下的index文件（.git/index）中，所以我们把暂存区有时也叫作索引（index）。
		版本库：工作区有一个隐藏目录.git，这个不算工作区，而是Git的版本库。


​		
		tips:Mac OS X上，如果需要查看.git目录下的隐藏文件，操作很简单： 
		做法是：打开一个Terminal终端窗口，输入：
		
		defaults write com.apple.finder AppleShowAllFiles TRUE
		然后重启Finder，输入：
		killall Finder
		
		如果你完成了需要的操作，恢复隐藏设置，同样打开Terminal终端窗口，输入：
		defaults write com.apple.finder AppleShowAllFiles FALSE
		然后重启Finder，输入：
		killall Finder
		
	1 创建版本库：
		
		1.1 创建空目录
			mkdir learngit 创建空目录
			cd learngit 进入到目录里
			pwd 显示当先目录
			
		1.2 git init  通过git init命令把这个目录变成Git可以管理的空仓库：
	2 把文件添加到版本库
	
		1.1 用命令git add告诉Git,实际上就是把文件修改添加到暂存区
			git add readme.txt [如何一下添加所有文件，git add .]
			执行上面的命令，没有任何显示，没有消息就是好消息，说明添加成功。
		
		1.2	用命令git commit告诉Git，实际上就是把暂存区的所有内容提交到当前分支。
			git commit -m "wrote a readme file"
			
		1.3 版本回退
			git log 命令显示从最近到最远的提交日志
			git reset --hard HEAD^  回退到上一个版本
			git reset --hard 1094a（commit）回退到某个版本
			git reflog  用来记录你的每一次命令
			git status 查看文件状态，有没有修改
			git checkout -- file  丢弃工作区的修改
			rm test.txt 删除这个test文件
			git rm test.txt 版本库中删除该文件  
			
			git remote add origin git@github.com:wuhaijun/learngit.git 本地关联的就是我的远程库
			git push -u origin master	把本地库的所有内容推送到远程库上
				由于远程库是空的，我们第一次推送master分支时，加上了-u参数，
				Git不但会把本地的master分支内容推送的远程新的master分支，
				还会把本地的master分支和远程的master分支关联起来，
				在以后的推送或者拉取时就可以简化命令。
			ssh-keygen -t rsa -C "youremail@example.com"  创建SSH Key
				
		1.4	从远程库克隆
		
			git clone git@github.com:wuhaijun/learngit.git
			
			提取远程仓库 git fetch   
						git merge
			删除远程仓库
						git remote rm [别名]
			查看远程仓库
						git remote -v
			
		1.5	分支管理
			1.5.1 git branch dev	创建分支
				  git checkout dev  切换到分支 或者 git switch dev
				  git checkout -b dev 创建并切换到分支 或 git switch -c dev
			1.5.2 git merge dev 把dev分支的工作成果合并到master分支上
			1.5.3 git branch -d dev 删除分支dev  git branch -D dev 强行删除dev
			1.5.4 git branch 查看分支
			
		1.6	解决冲突
		
			创建分支并切换到dev1上
				git checkout -b dev1
			修改readme.txt最后一行，改为：
				Creating a new branch is quick AND simple.
			
			提交dev1修改
			git add readme.txt
			git commit -m "AND simple"
			
			切换分支到master
				git checkout master
			在master分支上把readme.txt文件的最后一行改为：
				Creating a new branch is quick & simple.
				
			提交master修改
			git add readme.txt 
			git commit -m "& simple"
			
			将dev1合并到master
			git merge dev1 
			
			修改同一个地方会有冲突
			冲突如下形式：
			<<<<<<< HEAD
			Creating a new branch is quick & simple.
			=======
			Creating a new branch is quick AND simple.
			>>>>>>> 
			
			将冲突解决后 并提交
			git add readme.txt 
			git commit -m "conflict fixed"
			
			看到分支的合并情况
			git log --graph --pretty=oneline --abbrev-commit
			
			最后在删除分支	dev1
			git branch -d dev1
		1.7 分支策略
				在实际开发中，我们应该按照几个基本原则进行分支管理：
				首先，master分支应该是非常稳定的，也就是仅用来发布新版本，平时不能在上面干活；
				那在哪干活呢？干活都在dev分支上，也就是说，dev分支是不稳定的，到某个时候，比如1.0版本发布时，再把dev分支合并到master上，在master分支发布1.0版本；
				你和你的小伙伴们每个人都在dev分支上干活，每个人都有自己的分支，时不时地往dev分支上合并就可以了


​			
​			
​		 
​		 
​		 
​		 
​		
​		
​	
