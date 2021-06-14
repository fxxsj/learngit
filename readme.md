mkdir learngit 创建一个文件夹
cd learngit 进入该文件夹
pwd 显示当前目录

git init 通过该命令把这个目录变成 git 可以管理的仓库

git add 把文件添加到仓库

git commit 把文件提交到仓库 -m 后面输入其次提交的说明 有参数可以不这么做，但对自已或别人的阅读不友好

小结
现在总结一下今天学的两点内容：

初始化一个Git仓库，使用git init命令。

添加文件到Git仓库，分两步：

使用命令git add <file>，注意，可反复多次使用，添加多个文件；
使用命令git commit -m <message>，完成。

------

git status 命令掌握仓库当前的状态

git diff 查看具体修改了什么内容

小结
要随时掌握工作区的状态，使用git status命令。

如果git status告诉你有文件被修改过，用git diff可以查看修改内容。

------

git log 查看历史记录

git log --pretty=oneline 简化输出信息

Git必须知道当前版本是哪个版本，在Git中，用HEAD表示当前版本，也就是最新的提交1094adb...（注意我的提交ID和你的肯定不一样），上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100。

git reset --hard参数有啥意义？

git reflog 用来记录你的每一次命令

小结
HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id。

穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。

要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。