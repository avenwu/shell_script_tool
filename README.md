#btool
This shell script tool contains a set of commands which make it easy to operate one's git repo(Keep in mind it's a shell script which only supports shell terminal, cmd on windows is not available).

###Installation
> -Download this project(only btool & .babytree are necessary);

> -Copy the .babytree & btool to one of your local directory and add it system envirenment path;

> -Custom the .babytree as you like

> -Test the btool with ./btool or btool. Then the usgae introduction should displayed. 

###Usage
Use btool help for detailed usage introduction, here are some usgae examples:



1. btool co hello 
Checkout new branch, eg:141015\_nameHello\_dev

2. btool pull
git pull all the configured projects

3. btool push
generate diff file for arc to upload; push your working branch to remote git repo

###Workflow
Update project frequently is kind of boring, use `btool pull` to save your life, it will update all projects at the same time. No need to find our project directorys everytime we'd like to update one project.
Once we decide to make a change of the code, use `btool co yourBranch ` to checkout new branch. Then you may edit your project with any IDE as you like and commit the changes with normal git commands such as:git add/commit; After these make review request and push branch to remote repo with `btool push`

------
#btool
btool脚本包含几个常用的命令，主要用来简化开发中的git版本操作（此脚本为shell脚本，可以在git bash/terminal执行，不可以在cmd内使用）。

###安装
> -下载项目(只有btool和.babytree 是必须的文件);

> -配置脚本，将.babytree和btool 拷贝到本地目录中，并将目录添加到系统环境变量（window/*nix的有各自的添加方式和安装jdk一样）;

> -.babytree用于配置个人信息，具体参见内部说明

> -执行脚本./btool或 btool，终端将提示使用说明

###使用说明
终端内输入 btool help可以查看使用说明，下面试几个简单示例:


1. btool co hello 
切分支, eg:141015\_nameHello\_dev

2. btool pull
拉取远程代码到本地（目录无关，可以在任意目录执行，将同步.babytree中配置好的项目）

3. btool push
生成差异文件，借由arc diff上传至review地址，成功后自动推送开发分支到版本库对应分支

###开发流程
每次同步项目是一件很枯燥的事，使用常规git操作我们必须先找到每个项目然后使用git fetch/pull等操作，现在可以使用btool pull进行简化，在任意位置执行该命令，将一次性同步所有配置好的项目

