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
