# **Git版本控制工具**

# 一、**版本控制[问题引入]**

## （一）**版本控制思想**

从个人工作和团队协作两个方面（角度）介绍版本控制思想

n 个人工作

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps251.jpg) 

往往为了恢复到某一个版本，我们不停的对我们的文件进行复制修改（备份）

n 团队协作

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps252.jpg) 

版本从何而来呢？

设定场景：

SVN以自增数字编写版本号，如123

Git，以hash码来标记每个不同的版本

A提交一次代码，服务器的版本为1

B提交一次代码，服务器的版本为2

…

每提交一次代码，服务器的文件版本+1，这样每次提交的东西都有一个版本号对应，易于管理，所以这种软件就叫做版本控制软件。安装了版本控制软件的服务器叫做，版本控制服务器，作用：团队协作开发。文件上传到版本控制服务器，仅有文件内容还不够，还需要文件的元数据信息（描述数据的数据就叫做元数据）（修改时间、修改人、备注注释信息等），这样才能够便于恢复版本、追责等

 

## （二）**版本控制软件应该具有的功能**

l 协同修改
多人并行不悖的修改服务器端的同一个文件。

l 数据备份
不仅保存目录和文件的当前状态， 还能够保存每一个提交过的历史状态。

l 版本管理

在保存每一个版本的文件信息的时候要做到不保存重复数据，以节约存储空
间，提高运行效率。这方面 SVN 采用的是增量式管理的方式，而 Git 采取了文
件系统快照的方式

l 历史记录
查看修改人、 修改时间、 修改内容、 日志信息。
将本地文件恢复到某一个历史状态。

l 分支管理
允许开发团队在工作过程中多条生产线同时推进任务， 进一步提高效率。

注意：版本控制不仅适用于IT领域

## （三）**版本控制工具介绍**

1、集中式版本控制工具

代表：**cvs、svn、vss**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps253.jpg) 

弊端：容错性不好，服务器宕机、磁盘坏掉都会影响工作进度

 

2、分布式版本控制工具

代表性：git、BitKeeper

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps254.jpg) 

# 二、**Git介绍[了解]**

## （一）**Git简史**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps255.jpg) 

## （二）**Git官网和Logo**

官网地址：<https://git-scm.com/>

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps256.jpg) 

## （三）**Git的优势**

1. 大部分操作在本地完成，不需要联网（不折不扣的分布式）

2. 完整性保证

3. Hash算法

4. 尽可能添加数据而不是删除或修改数据

5. 分支操作非常快捷流畅

6. 与 Linux 命令全面兼容


# 三、**Git工作流程[了解]**

一般工作流程如下：

1．从远程仓库中克隆 Git 资源作为本地仓库。

2．从本地仓库中checkout代码然后进行代码修改。

3．在提交前先将代码提交到暂存区。

4．提交修改。提交到本地仓库。本地仓库中保存修改的各个历史版本。

5．在修改完成后，需要和团队成员共享代码时，可以将代码push到远程仓库。

下图展示了 Git 的工作流程：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps257.jpg)

# 四、**Git的安装[应用]**

最早Git是在Linux上开发的，很长一段时间内，Git也只能在Linux和Unix系统上跑。不过，慢慢地有人把它移植到了Windows上。现在，Git可以在Linux、Unix、Mac和Windows这几大平台上正常运行了。由于开发机大多数情况都是windows，所以本教程只讲解windows下的git的安装及使用。

## （一）**软件下载**

下载地址：<https://git-scm.com/download>

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps258.jpg) 

## （二）**软件安装[应用]**

### 1．**安装git for windows**

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps259.jpg) 

一路“下一步”使用默认选项即可。注意：安装路径不要用中文

验证安装是否成功：在任何一个目录下右键看是否有菜单

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps260.jpg) 

### 2．**安装TortoiseGit**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps261.jpg) 

一路“下一步”使用默认选项即可。

默认选项下会启动配置画面：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps262.jpg) 

由于目前只有英文语言包，默认即可继续下一步。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps263.jpg) 

配置git.exe，在4.2.1中已经安装过git-for-windows了所以在此找到git.exe所在的目录。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps264.jpg) 

配置开发者姓名及邮箱，每次提交代码时都会把此信息包含到提交的信息中。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps265.jpg) 

使用默认配置，点击“完成”按钮完成配置。

完整完毕后在系统右键菜单中会出现git的菜单项。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps266.jpg) 

### 3．**安装中文语言包**

安装中文语言包并不是必选项。可以根据个人情况来选择安装。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps267.jpg) 

直接“下一步”完整完毕。

语言包安装完毕后可以在TortoiseGit的设置中调整语言

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps268.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps269.jpg) 

# 五、**Git的结构[认识]**

## （一）**Git的本地结构**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps270.jpg) 

## （二）**Git的代码托管中心**

代码托管中心的任务：维护远程库

1. 局域网环境下：GitLab服务器

2. 外网环境下：GitHub、码云


## （三）**本地库和远程库**

本地库和远程库的交互方式，介绍这么两种：一种是团队内部协作，一种是跨团队协作

# 六、**Git命令行操作[掌握]**

Git本地项目仓库(可以多个)初始化

命令行操作学习路线：初始化git本地版本库——>在本地版本库管理文件（新建文件 —>把文件加入git的管理 —> 修改文件 —> 恢复到之前某一个版本）

## （一）**创建版本库**

### 1．**使用GitBash**

在当前目录中点击右键中选择Git Bash来启动。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps273.jpg)![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps274.jpg) 

创建仓库执行命令：

n 命令：git init

n 效果

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps275.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps276.jpg) 

注意：.git目录中存放的是本地库相关的子目录和文件，不要删除，也不要胡乱修改

### 2．**使用TortoiseGit**

使用TortoiseGit时只需要在目录中点击右键菜单选择“在这里创建版本库”

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps277.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps278.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps279.jpg) 

版本库创建成功，会在此目录下创建一个.git的隐藏目录，如下所示：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps280.jpg) 

在windows中如何显示隐藏目录隐藏目录请自行百度o(╯□╰)o

**概念：**

**版本库：“.git”目录就是版本库，将来文件都需要保存到版本库中。**

**工作目录：包含“.git”目录的目录，也就是.git目录的上一级目录就是工作目录。只有工作目录中的文件才能保存到版本库中。**

## （二）**设置签名**

**形式**

用户名：tom

Email地址：[helloword@aliyun.com](mailto:helloword@aliyun.com)

**作用**：区分不同开发人员的身份

**辨析**：这里设置的签名和登录远程库(代码托管中心)的账号、 密码没有任何关
系

**命令**：

项目级别/仓库级别：仅在当前本地库范围内有效

git config user.name tom_pro

git config user.email [helloword@aliyun.com](mailto:helloword@aliyun.com)

l 信息保存位置：.git/config文件
![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps281.jpg)

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps282.jpg) 

**系统用户级别**：登录当前操作系统的用户范围

git config --global user.name tom_global

git config --global user.email [tomabc@aliyun.com](mailto:tomabc@aliyun.com)

信息保存位置：保存在当前仓库目录下的 .git/config 文件中

 

**级别优先级**：

就近原则：项目级别优先于系统用户级别，二者都有时采用项目级别的签名

如果只有系统用户级别的签名，就以系统用户级别的签名为准

二者都没有不允许

## （三）**基本操作**

### 1．**添加**

**使用GitBash**

​	git add [filename]

​	将工作区的“新建/修改”添加到暂存区

在~/Desktop/gittest目录下创建一个good.txt文件

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps283.jpg) 

 

使用TortoiseGit

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps284.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps285.jpg) 

### 2．**提交**

**使用GitBash**

​	git commit -m “commit message” [file name]

​	将暂存区的内容提交到本地库（暂存区内容修改后进行提交）

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps286.jpg) 

使用TortoiseGit

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps287.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps288.jpg) 

### 3．**查看历史记录**

**使用GitBash**

​	git log

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps289.jpg) 

​		git log --pretty=oneline 美化log日志

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps290.jpg) 

​		git log --oneline 美化log日志

​		![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps291.jpg)

git reflog**（推荐）** 用来恢复本地错误操作很重要的一个命令 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps292.jpg) 

HEAD@{移动到当前版本需要多少步}

使用TortoiseGit

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps293.jpg) 

### 4．**状态查看**

**使用GitBash**

​	git status

​	查看工作区，暂存区状态

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps294.jpg) 

文件名红色表明工作目录中的文件尚未被追踪管理

**前进后退**

本质：其实内部维护了一个HEAD指针，做这么一个reset操作的时候，其实相当于移动了HEAD指针（表明的是当前的状态）

**基于索引值操作**[推荐]

git reset --hard [局部索引值/版本号前缀]

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps295.jpg) 

使用^符号：只能后退

git reset --hard HEAD^ 一个表示后退一步，n个表示后退n步

使用~符号：只能后退

git reset --hard HEAD~n（注：表示后退n步）

### 5．**删除文件**

使用TortoiseGit

需要删除无用的文件时可以使用git提供的删除功能直接将文件从版本库中删除。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps296.jpg) 

注意:不要仅仅从工作目录删除，删除之后也需要git add然后git commit提交到本地仓库管理

### 6．**删除文件并找回**

**使用GitBash**

前提：删除前，文件存在时的状态提交到了本地库

操作：git reset --hard 指针位置

删除操作已经提交到本地库：指针位置指向历史记录

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps297.jpg) 

### 7．**比较文件差异**

**使用GitBash**

git diff [文件名]：将工作区中的文件和暂存区进行比较

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps298.jpg) 

git diff 本地仓库中的历史版本 文件名：将工作区中的文件和版本库进行比较(主要)

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps299.jpg) 

使用TortoiseGit

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps300.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps301.jpg) 

### 8．**还原修改**

使用TortoiseGit

当文件修改后不想把修改的内容提交，还想还原到未修改之前的状态。此时可以使用“还原”功能

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps302.jpg)![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps303.jpg)![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps304.jpg) 

**注意：此操作会撤销所有未提交的修改，所以当做还原操作是需要慎重慎重！！！**

## （四）**工作区和暂存区**

Git和其他版本控制系统如SVN的一个不同之处就是有暂存区的概念。

什么是工作区（Working Directory）？

工作区就是你在电脑里能看到的目录，比如我的reporstory文件夹就是一个工作区。

有的同学可能会说repository不是版本库吗怎么是工作区了？其实repository目录是工作区，在这个目录中的“.git”隐藏文件夹才是版本库。这回概念清晰了吧。

**Git的版本库里存了很多东西，其中最重要的就是称为stage（或者叫index）的暂存区，还有Git为我们自动创建的第一个分支master，以及指向master的一个指针叫HEAD。**

如下图所示：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps305.png)

分支和HEAD的概念我们稍后再讲。前面讲了我们把文件往Git版本库里添加的时候，是分两步执行的：

第一步是用git add把文件添加进去，实际上就是把文件修改添加到暂存区；

第二步是用git commit提交更改，实际上就是把暂存区的所有内容提交到当前分支。

因为我们创建Git版本库时，Git自动为我们创建了唯一一个master分支，所以，现在，git commit就是往master分支上提交更改。

你可以简单理解为，需要提交的文件修改通通放到暂存区，然后，一次性提交暂存区的所有修改。

## （五）**案例：将java工程提交到版本库**

**使用TortoiseGit**：

第一步：将参考资料中的java工程gittest复制到工作目录中

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps306.jpg) 

第二步：将工程添加到暂存区。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps307.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps308.jpg)![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps309.jpg) 

点击确定完成暂存区添加。

三、忽略文件或文件夹

在此工程中，并不是所有文件都需要保存到版本库中的例如“.idea”目录及目录下的文件就可以忽略。好在Git考虑到了大家的感受，这个问题解决起来也很简单，在Git工作区的根目录下创建一个特殊的.gitignore文件，然后把要忽略的文件名填进去，Git就会自动忽略这些文件。

如果使用TortoiseGit的话可以使用菜单项直接进行忽略。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps310.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps311.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps312.jpg)![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps313.jpg) 

选择保留本地文件。完成后在此文件夹内会多出一个.gitignore文件，这个文件就是文件忽略文件，当然也可以手工编辑。其中的内容就是把.idea目录忽略掉。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps314.jpg) 

四、提交代码

将代码添加到master分支上，其中.gitignore文件也需要添加到暂存区，然后提交到版本库。

## （六）**忽略文件语法规范**

空行或是以 # 开头的行即注释行将被忽略。

可以在前面添加正斜杠 / 来避免递归,下面的例子中可以很明白的看出来与下一条的区别。

可以在后面添加正斜杠 / 来忽略文件夹，例如 build/ 即忽略build文件夹。

可以使用 ! 来否定忽略，即比如在前面用了 *.apk ，然后使用 !a.apk ，则这个a.apk不会被忽略。

\* 用来匹配零个或多个字符，如 *.[oa] 忽略所有以".o"或".a"结尾， *~ 忽略所有以 ~ 结尾的文件（这种文件通常被许多编辑器标记为临时文件）； [] 用来匹配括号内的任一字符，如 [abc] ，也可以在括号内加连接符，如 [0-9] 匹配0至9的数； ? 用来匹配单个字符。 

看了这么多，还是应该来个栗子：

\# 忽略 .a 文件

*.a

\# 但否定忽略 lib.a, 尽管已经在前面忽略了 .a 文件

!lib.a

\# 仅在当前目录下忽略 TODO 文件， 但不包括子目录下的 subdir/TODO

/TODO

\# 忽略 build/ 文件夹下的所有文件

build/

\# 忽略 doc/notes.txt, 不包括 doc/server/arch.txt

doc/*.txt

\# 忽略所有的 .pdf 文件 在 doc/ directory 下的

doc/**/*.pdf

# 七、**Git分支管理[了解]**

往往应用于大型项目，而且分支由项目经理管理

## （一）**什么是分支**

在版本控制过程中，使用多条线同时推进多个任务

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps315.jpg) 

## （二）**分支的好处**

各个分支在开发过程中，如果某一个分支开发失败，不会对其他分支有任何影响，失败的分支删除重新开始即可

## （三）**分支操作**

### 1．**创建分支**

**使用GitBash**

git branch 分支名

使用TortoiseGit

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps316.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps317.jpg) 

如果想创建完毕后直接切换到新分支可以勾选“切换到新分支”选项或者从菜单中选择“切换/检出”来切换分支：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps318.jpg) 

 

### 2．**查看分支**

**使用GitBash**

git branch -v

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps319.jpg) 

### 3．**切换分支（checkout检出）**

**使用GitBash**

 

git checkout 【分支名】

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps320.jpg) 

 

### 4．**合并分支**

**使用GitBash**

第一步：切换到接受修改的分支

git checkout 【被合并分支名】

第二部：执行merge（合并）命令

git merge 【有新内容分支名】

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps322.jpg) 

### 5．**解决冲突**

**使用GitBash**

冲突的表现及冲突的解决

第一步：编辑文件，删除特殊符号

第二步：把文件修改到满意的程度，保存退出

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps323.jpg) 

不要留有特殊字符<<<<<<< =>>>>>>

第三步：git add 文件名

第四步：git commit -m ‘日志信息’，注意此时，commit一定不能带具体的文件名,否则会出现错误

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps324.jpg) 

# 八、**GitHub[应用]**

## （一）**添加远程仓库**

现在我们已经在本地创建了一个Git仓库，又想让其他人来协作开发，此时就可以把本地仓库同步到远程仓库，同时还增加了本地仓库的一个备份。常用的远程仓库就是github：<https://github.com/>，接下来我们演示如何将本地代码同步到github。

## （二）**账号信息**

GitHub首页就是注册页面：<https://github.com/>

首先你得在github上创建一个账号

| ![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps325.jpg) | Email地址：github[yuebuqun@aliyun.com](mailto:yuebuqun@aliyun.com)GitHub账号：githubyuebuqun |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps326.jpg) | Email地址：github[linghuchong@aliyun.com](mailto:linghuchong@aliyun.com)GitHub账号：githublinghuchong |
| ![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps327.jpg) | Email地址：github[dongfangbubai@aliyun.com](mailto:dongfangbubai@aliyun.com)GitHub账号：githubdongfangbubai |

## （三）**创建GitHub远程库**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps328.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps329.jpg) 

点击“create repository”按钮仓库就创建成功了。

Github支持两种同步方式“https”和“ssh”。如果使用https很简单基本不需要配置就可以使用，但是每次提交代码和下载代码时都需要输入用户名和密码。如果使用ssh方式就需要客户端先生成一个密钥对，即一个公钥一个私钥。然后还需要把公钥放到githib的服务器上。这两种方式在实际开发中都用应用，所以我们都需要掌握。

## （四）**创建远程仓库地址别名**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps330.jpg) 

git remote -v 查看当前所有远程地址别名

git remote add [别名] [远程地址]

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps331.jpg) 

## （五）**同步到远程仓库**

**https方式**

git push [别名] [分支名]

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps332.jpg) 

**SSH方式**

git remote rm origin

git remote add origin [ssh仓库地址]

git push -u origin [分支]

## （六）**从远程仓库克隆**

命令：git clone [仓库远程地址]

效果：

1. 完整的把远程库下载到本地

2. 创建origin远程地址别名

3. 初始化本地库


使用TortoiseGit：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps333.jpg) 

## （七）**团队成员邀请**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps334.jpg) 

 

复制邀请连接

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps335.jpg) 

​	“岳不群”其他方式把邀请连接发送给“令狐冲”，“令狐冲”登录自己的GitHub账号，访问邀请连接，接受邀请

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps336.jpg) 

## （八）**从远程仓库取代码**

pull = fetch（获取的意思） + merge

git fetch [远程库地址别名] [远程分支名]

如果要查看，需要切换仓库git checkout origin/master,然后cat 文件

例如：

git fetch original master

git checkout original/master

cat ….txt

git checkout master

git merge original/master

git merge [远程库地址别名/远程分支名]

git pull [远程库地址别名] [远程分支名]

或

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps337.jpg) 

## （九）**解决冲突**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps338.jpg) 

首先需要pull最新的代码

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps339.jpg) 

然后处理冲突，和分支合并处理冲突一样，注意commit时不要带文件名，commit后push到远程

**要点：**

1. 如果不是基于GitHub远程库的最新版所做的修改，不能推送，必须先拉取

2. 拉取下来如果进入冲突状态，模仿分支冲突解决即可


## （十）**跨团队协作**

1. 把项目的地址发送给团队外部的人（线下发送）

2. 团队外部人员登录github，然后访问给出的地址

3. 团队外人员把fork后的远程仓库clone到本地进行fork


![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps340.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps341.jpg) 

团队外人员本地编辑提交，push到远程

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps342.jpg) 

 pull request

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps343.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps344.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps345.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps346.jpg) 

团队内人员，查看审核请求

团队人员登录

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps347.jpg) 

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps348.jpg) 

查看修改内容

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps349.jpg) 

n然后将远程库拉取到本地即可，拉取到本地结束跨团队协作的过程

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps350.jpg) 

## （十一）**SSH操作**

### 1．**什么是ssh?**

SSH 为 Secure Shell（安全外壳协议）的缩写，由 IETF 的网络小组（Network Working Group）所制定。SSH 是目前较可靠，专为远程登录会话和其他网络服务提供安全性的协议。利用 SSH 协议可以有效防止远程管理过程中的信息泄露问题。

### 2．**基于密匙的安全验证**

使用ssh协议通信时，推荐使用基于密钥的验证方式。你必须为自己创建一对密匙，并把公用密匙放在需要访问的服务器上。如果你要连接到SSH服务器上，客户端软件就会向服务器发出请求，请求用你的密匙进行安全验证。服务器收到请求之后，先在该服务器上你的主目录下寻找你的公用密匙，然后把它和你发送过来的公用密匙进行比较。如果两个密匙一致，服务器就用公用密匙加密“质询”（challenge）并把它发送给客户端软件。客户端软件收到“质询”之后就可以用你的私人密匙解密再把它发送给服务器。

#### （1）**ssh密钥生成**

在windows下我们可以使用 Git Bash.exe来生成密钥，可以通过开始菜单或者右键菜单打开Git Bash

 

   ![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps351.jpg)

git bash 执行命令,生命公钥和私钥

命令: **ssh-keygen -t rsa**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps352.jpg) 

执行命令完成后,在window本地用户.ssh目录C:\Users\用户名\.ssh下面生成如下名称的公钥和私钥:

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps353.jpg) 

 

#### （2）**ssh密钥配置**

密钥生成后需要在github上配置密钥本地才可以顺利访问。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps354.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps355.jpg) 

在key部分将id_rsa.pub文件内容添加进去，然后点击“Add SSH key”按钮完成配置。

### 3．**SSH原理**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps356.jpg) 

# 九、**Idea中操作Git[掌握]**

## （一）**在Idea中配置git**

安装好IntelliJ IDEA后，如果Git安装在默认路径下，那么idea会自动找到git的位置，如果更改了Git的安装位置则需要手动配置下Git的路径。

选择File→Settings打开设置窗口，找到Version Control下的git选项：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps357.jpg) 

选择git的安装目录后可以点击“Test”按钮测试是否正确配置。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps358.jpg) 

## （二）**将工程添加至git**

1）在idea中创建一个工程，例如创建一个java工程，名称为idea-git-test，如下图所示：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps359.jpg) 

2）创建本地仓库

在菜单中选择“vcs”→Import into Version Control→Create Git Repository...

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps360.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps361.jpg) 

选择工程所在的上级目录。本例中应该选择idea-projects目录，然后点击“OK”按钮，在工程的上级目录创建本地仓库，那么idea-projects目录就是本地仓库的工作目录，此目录中的工程就可以添加到本地仓库中。也就是可以把idea-git-test工程添加到本地仓库中。

选择之后在工具栏上就多出了git相关工具按钮：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps362.jpg) 

 

3）将工程添加至本地仓库

直接点击![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps363.jpg)commit按钮，将工程提交至本地仓库。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps364.jpg) 

然后点击“commit”按钮，将工程添加至本地仓库。

4）推送到远程

在github上创建一个仓库然后将本地仓库推送到远程。

在工程上点击右键，选择git→Repository→push，

或者在菜单中选择vcs→git→push

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps365.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps366.jpg) 

点击“Define remote”链接，配置https形式的URL，git形式的无法通过。然后点击OK

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps367.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps368.jpg) 

点击“push”按钮就讲本地仓库推送到远程，如果是第一次配置推送需要输入github的用户名和密码。

## （三）**从远程仓库克隆**

关闭工程后，在idea的欢迎页上有“Check out from version control”下拉框，选择git

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps369.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps370.jpg) 

此处仍然推荐使用htts形式的url，点击“test”按钮后显示连接成功。

点击OK按钮后根据提示将远程仓库克隆下来，然后倒入到idea中。

## （四）**从服务端拉取代码**

如果需要从服务端同步代码可以使用工具条中的“update”按钮

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps371.jpg) 

# 十、**Git基本原理[了解]**

## （一）**哈希**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps372.jpg) 

哈希是一个系列的加密算法，各个不同的哈希算法虽然加密强度不同，但是有以下几个共同点：

1. 不管输入数据的数据量有多大，输入同一个哈希算法，得到的加密结果长度固定

2. 哈希算法确定，输入数据确定，输出数据能够保证不变

3. 哈希算法确定，输入数据有变化，输出数据一定有变化，而且通常变化很大

4. 哈希算法不可逆

5. Git底层采用的是SHA-1算法


哈希算法可以被用来验证文件，原理如下图所示

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps373.jpg) 

## （二）**Git保存版本的机制**

集中式版本控制工具的文件管理机制：
以文件变更列表的方式存储信息。系统将它们保存的信息看作是一组基本文件和每个文件随时间逐步累积的差异。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps374.jpg) 

Git的文件管理机制

​	Git把数据看作是小型文件系统的一组快照。每次提交更新时Git都会对当前的全部文件制作一个快照并保存这个快照的索引。为了高效，如果文件没有修改，Git不再重新存储该文件，而是只保留一个连接指向之前存储的文件。所以Git的工作方式可以称之为快照流

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps375.jpg) 