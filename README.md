# git使用




	git config --global user.name "username"
	git config --global user.email "email@.com"
配置用户信息


	git init
初始化git；创建一个.git文件夹
或使用

	git clone http://github.com/name/name 
克隆一个文件夹

------------


	git status
	
	
查看暂存区目录
- 未暂存标红
- 暂存但未commit标绿




	git add 文件名
	git add .          //全部文件
	git add *.txt      //通配符



添加文件到暂存区



	git commit -m "COMMIT注释"
为上传的文件标注


	git log
查看提交修改记录

	git reset HEAD <版本号>
回档到某一版本 （版本号为40位16进制）

# github
- 使用ssh


	ssh-keygen -t rsa -C "youremail@example.com"

创建一个ssh秘钥 在~/.ssh文件夹打开 id_rsa.pub
复制粘贴到github  Account => Settings =>ssh

	ssh -T git@github.com
用此命令验证
使用ssh好处是不用每次上传都输密码

- 提交到github


	 git remote add origin git@github.com:camera-2018/testgit2.git
会在 \.git\config 文件里加进名称为origin的网址



	 git push origin master 

推送到github
