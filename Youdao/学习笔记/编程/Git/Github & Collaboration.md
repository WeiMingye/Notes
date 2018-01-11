# Github & Collaboration
## 使用远程仓库
### 始终使用特性分支
记住，使用具有描述性的分支进行commmit非常有用。分支有助于隔离不相关的更改。所以，当与其他开发者协助时，确保创建一个新的分支，并使用描述性的名称说明它所包含的更改。

### git remote命令
- git remote add orgin https/ssh 与远端建立连接 （即可用orgin代替https/ssh）
- git remote -v 详细查看所有远端仓库

### git push命令
- git push [remote-shortname] [branch] 用于将本地分支推送到远端分支

### fetch命令
git fetch 用于从远程仓库分支检索 commit ，但不会在收到这些 commit 之后，自动将本地分支与远程跟踪分支合并。   

运行 git fetch 后，会发生以下活动：
- 远程分支上的commit会复制到本地仓库
- 本地跟踪分支（例如，origin/master）移到指向最新的 commit  

使用fetch而不是pull的情形就是，当远程仓库的commit与本地的commmit有冲突时，这是使用pull就会失效，而是需要将远程仓库的commit fetch下来，然后将origin/master（即本地追踪分支）与本地分支手动解决冲突合并后再push回远程仓库  

命令 | 用途
--- | ---
git fetch | 把远程仓库的所有分支的commit都取回以更新远程追踪分支
git fetch next | 远程仓库的next分支的commit取回更新本地远程追踪分支


### git push命令
命令 | 用途
--- | ---
git pull <remote-shortname> <remote-branch>:<local-branch> | 将远端仓库的分支的更新与本地的分支同步
git pull <r-s> <r-b> | 将远端仓库分支的更新与当前分支同步
git pull <r-s> | 将远端仓库与本地“追踪分支”同步
git pull | 将唯一远端仓库的“追踪分支”同步


## 使用其他开发者的仓库
### fork仓库
当使用`git clone`克隆他人的仓库时，本地无法push因为这个仓库并 不属于你    

这时可以使用fork在远程克隆他人的仓库，然后在pull回本地便可拥有所有权  
### 查看现有工作
当项目有多人参与协作时，可以使用`git log`的相关命令进行筛选显示    

命令 | 用途
--- | ---
git shortlog | 查看每位贡献者的coomit
git shortlog -s -n| 查看每位贡献者的coomit,-s仅显示数量 -n按数量进行排序
git shortlog --author=Wei | 仅显示名字以Wei开头的作者的commit
git shortlog --author='Wei Mingye' | 显示Wei Mingye作者的commit
git log --oneline grep="css" (or grep css) | 筛选内容为css的commit

### 确认工作
1. 在开始任何工作之前，阅读项目的CONTRIBUTING.md文件   
2. 查看项目上Github的问题：
    1. 查看现有问题，看是否有相似想法的更改避免重复工作
    2. 若没有重复的更改，可以创建一个新的issue
    3. 与项目维护者交流想要作出的更改  

3. 当开始开发后，将所有工作commit到特性分支上：
    1. 不要在主分支上工作
    2. 确保给特性分支赋予一个清晰、描述性的名称

4. 编写commit的一些建议：
    1. 精度足够小的commmit，便于精细给予建议和评价
    2. 使用清晰、具有描述性的提交说明
    3. 在大改动的情况下，考虑更新README文件

## 参与项目协助
### 创建PULL Rrequest
PULL Request就是请求让源仓库拉取你的commit，并融合在其项目中。要创建Pull Request，一般要：   
1. fork源仓库
2. 将fork仓库克隆到你的计算机
3. 进行一些commit（最好在特性分支上！）
4. 将commit推送回你的fork（只有从自己github clone下来的才可以push）
5. 创建一个新的Pull Request， 并选择包含你的新commit的分支

### 与源项目保持同步
当你在fork的项目副本上工作时，源项目有可能已经添加了新的更改，因此你需要将你fork的副本与源项目保持同步，将源仓库的更改提取到你fork副本上，你需要：
1. 获取源仓库可克隆的URL
2. 使用`git remote add`命令创建一个新的远程仓库连接
    1. 一般使用简写名upstream指向源仓库
    2. 提供源仓库的URL
    3. 这时，upstream就代表本地对源仓库的追踪分支
3. 活鱼新的upstream远程仓库
4. 将upstream的分支合并到本地分支
5. 将更新的本地分支推送到你的origin仓库

### 与项目维护者的交流
如果项目维护者要求更改 Pull Request，则：

- 在你的 Pull Request 所基于的本地仓库的同一分支上添加一些必要 commit
- 将该分支推送到你的源仓库 fork 副本

### 压制commit
`git rebase`命令很强大，可以压制commit、修改commit等等  

可在使用rebase的时候先创建一个backup分支，当rebase效果不满意的时候可以回退  

#### rebase命令： `git rebase -i HEAD~3`   
`git rebase`命令会使commit移动到一个新的基底上（base）。在上述命令中，将以HEAD\~3作为基底，编辑其后面的HEAD\~2、HEAD\~1、HEAD

-i意味着将以交互模式下执行rebase，一开始建议使用交互模式执行rebase

#### 强制推送
当将合并后的commit推送时，github会试图阻止push，因为其担心会意外删除commit。注意使用git rebase编辑后的commit会具有一个新的SHA，相当于基底后的commit都被删除了  

使用`git push -f`强制推送commit  

若已经推送了想变基的commit，最好不要变基，因为若变基，基底后的commit都会发生改变，这将使得从你fork的仓库副本不一致，从基底后的commit都发生了变化，这将影响到其他开发者的工作

rebase命令 | 用途
--- | ---
p(pick) | 使commit保持原样
r(reword) | 保留commit内容，修改commit说明
e(edit) | 修改commit内容
s(squash) | 将commit的修改整合到之前的commit中
f(fixup) | 类似于squash，但删除提交说明
x(exec) | 运行shell命令
d(drop) | 删除commit