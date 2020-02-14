# test
test for learning new things
用来学习GitHub创建的第一个项目，试着记录一些学习的小tips......

### step1：创建一个文件夹
用来存放项目文件 mkdir XXX(文件夹名称）
### step2：切换到文件夹目录下
cd XXX
### step3:初始化git仓库
git init
### step4:生成SSH key
ssh-keygen -t rsa，然后Windows是在C:\Users\Administrator\.ssh 文件夹内找到 id_rsa.pub
### step5：到GitHub添加SSH key
### step6：验证是否添加成功
ssh -T  git@github.com




### 踩到的坑
1、Administrator@USER-5584O6AUGT MINGW64 ~/test (master)
$ git pull origin master
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

--- 解决方法
$ git remote add origin git@github.com:JingMandy/test.git

2、$ git push origin master
Warning: Permanently added the RSA host key for IP address '13.250.177.223' to the list of known hosts.
Everything up-to-date
--- 解决方法
$ git status
$ git add test.md
$ git config --global user.email "you@example.com"
$ git config --global user.name "Your Name"
$ git commit -m 'first commit'
$ git push origin master


3、$ git commit

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Administrator@USER-5584O6AUGT.(none)')
--- 解决方法
$ git config --global user.email "xxx@163.com"
$ git config --global user.name "用户名"




