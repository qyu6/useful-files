#### (2022.7.28更新)

返回上级目录
cd ..

进入到某级目录
code xx

显示当前路径
pwd

清屏
clear

列出当前路径下文件
ls

列出文件的详细信息
ls -l

列出路径下所有的文件，包含隐藏文件
ls -a

创建一个文件夹目录
mkdir xx

创建一个新文件
touch xx.xx

移除一个文件
rm xx.xx

移除一个文件夹
rm -r xx

强制移除某个文件或文件夹
rm -rf xx (never use "rm -rf", will delete everthing.)

* x1文件,x2文件夹：移动文件x1到文件夹x2\n'
'* x1文件夹,x2不存在,重命名文件夹x1为x2\n'
'* x1文件夹,x2文件夹,将文件夹x1移动到文件夹x2内
mv x1 x2

显示所有命令记录历史
history

显示帮助文档
help xx

退出bash环境
exit

显示当前git配置信息
git config -l

显示当前系统的git配置信息
git config --system --list

显示全局配置的内容，用户名+账户等，必须配置
git config --global --list

* git系统配置文件\n'
'* git全局配置文件路径
c:\program\files\git\etc\gitconfig\nc:\.gitconfig

设置用户名和邮箱-用户标识
git config --global --user.name "xx"\ngit config --global --user.email "xx"

显示git常用的命令
git

查看之前的版本历史信息
git log

简化git版本历史输出的信息
git log --pretty=online

在当前路径初始化一个git项目
git init

显示当前路径下所有文件的git状态
git status

将路径下所有文件添加到stage区
git add .

提交stage区的内容到本地仓库(如报错检查gitconfig信息)
git commit -m "<commit.message>"

将本地仓库内容同步到远程仓库
git push

将远程仓库克隆到本地
git clone <url>

将最新的远程仓库同步到本地
git pull

git忽略本地项目更改，直接用服务器版本来覆盖本地仓库
git fetch --all\ngit reset --hard origin/master\ngit pull

显示当前项目所有分支
git branch

显示所有远程分支
git branch -r

新建一个分支并停留在当前分支
git branch <branch.name>

新建一个分支并切换到该分支上
git checkout -b <branch.name>

转换工作区分支到新创建的分支上
git switch <branch.name>

如果remote仓库没有这个branch，则这个分支直接git push会无效，可以用这个命令来实现分支push
git push --set-upstream origin <branch.name>

合并指定分支到当前分支上
git merge <branch.name>

删除远程分支
git push origin --delete <branch.name>\ngit branch -dr <remote/branch>

显示当前路径下所有远程库
git remove -v

查看本机是否安装ssh
ssh

生成ssh公钥
ssh-keygen

使用加密算法生成公钥，一路回车;c:/admin/.ssh下回生成两个文件, .pub后缀的文件打开后，与Gitlab/Github绑定
ssh-keygen -t ras

git端验证绑定ssh是否成功
ssh -T git@github.com | ssh -T git@gitlab.com ..

输出所有git提交历史日志，查找要退回的版本
git log

进行版本回退操作
git reset --hard <commit_id>

回滚后推送至远程分支
git push origin

快捷命令，回退到上个版本
git reset --hard HEAD^ | HEAD^^-previous~previous

进入python交互模式
python -i

进入python终端命令行交互模式
winpty python

退出终端python交互模式
quit()

bash中运行.py文件，运行完成后停留在python终端环境
python -i xx.py

bash中运行.py文件，运行完成后退出python终端环境
winpty python xx.py