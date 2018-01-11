 # Udacity Git Note
 ## 显示commit
 命令 | 用途
 --- | ---
 git log | 显示commit
 git log --oneline | 简略显示commit
 git log --stat | 在commit下显示改变的行数
 git log -p（--patch） | 详细显示改变
 git log XXX SHA | 可显示SHA的commit
 git show | 仅显示最新的一个commit
 git reflog | 查看所有命令记录
 - 可在命令后添加commit的sha值以显示特定的commit
 

## 提交commit
命令 | 用途
--- | ---
git add <file1> ... <fileN> | 提交文件1到n
git add . | 提交当前目录以及所有嵌套文件到暂存区
git commit | 打开编辑器编辑注释提交
git commit -m “message” |绕过编辑器直接编辑提交
git diff | 查看已经放到暂存区但未提交的修改

### 建议
- 每一个方面的修改为一commit
- 消息篇幅简短（少于 60 个字符）

- 解释提交的作用（不是如何更改或为何更改！）

### 禁忌

- 请勿解释为何做出了这些更改（下文会深入讲解这一点）

- 请勿解释如何进行了更改（这是 git log -p 的目的！）

- 请勿使用单词"and"

- 如果你必须使用 "and"，则你的提交说明可能进行了太多的更改，将这些更改拆分为独立的 commit

例如 "make the background color pink and increase the size of the sidebar"

在编写提交说明时，我喜欢用以下短语造句："This commit will…"。你可以补充完整该句子并作为提交说明使用。

==最重要的是，在编写提交说明时保持一致性！==

### 忽略添加某些文件
- .gitignore 文件用来告诉 git 不应跟踪的文件
- 该文件应该放在 .git 目录所在的目录。
- 在.gitignore中可使用通配符

通配符  | 作用
------  | ------
空白行  | 空格
#       | 标记该行
*       | 匹配0个或多个字符
?       | 匹配一个字符
[abc]   | 匹配a或b或c
**      | 匹配嵌套目录（a/**/z:a/z或a/b//z或a/b/c/z）
.png    | 匹配扩展名为png的图片

## 标签、分支和合并
### 标签
命令 | 用途
--- | ---
git tag -a v1.0 | 打开编辑器编辑为最新的commit添加有说明的标签
git tag v1.1 | 为最新的commit添加没有说明的标签
git tag -a v1.0 a876543 | 向sha为a876543的commit添加标签
git log (--decorate) | 显示带有便签信息commit
git tag | 查看标签
git show [tagname] | 查看tabname的标签说明
git push origin [tagname] | 推送到远端
git push origin --tags | 推送全部未推送的标签  
git tag -d(--delete) v1.1 | 删除标签v1.1
git tag -d v0.9 + git push origin :refs/tags/v0.9 | 先删除本地再删除远端的标签

### 分支
命令 | 用途
--- | ---
git branch | 列出仓库中所有分支（只显示本地分支）
git branch -r | 列出远端仓库分支
git branch -a | 列出所有分支
git branch bname| 添加分支bname
git branch bname f24032df | 从f24032df处添加分支
git branch -d dname | 删除dname分支
git branch -D dname | 强制删除dname而无视dname新添的commmit
git checkout bname | 切换到bname分支，即改变HEAD指针
git checkout -b bname | 创建并且切换到分支bname
git log --oneline --decorate --grath --all | --graph以图形显示 --all 显示所有分支

### 合并分支
冲突指示符 | 意义
---------- | ----------
git merge <name-of-branch> |   合并分支
<<<<<<< HEAD | 此行下方的所有内容（直到下个指示符）显示了当前分支上的行
\|\|\|\|\|\|\|merged common ancestors |  此行下方的所有内容（直到下个指示符）显示了原始行的内容
======= | 表示原始行内容的结束位置，之后的所有行（直到下个指示符）是被合并的当前分支上的行的内容
>>>>>>> heading-update | 是要被合并的分支（此例中是 heading-update 分支）上的行结束指示符

## 撤销更改
命令 | 用途
--- |---
git commit --amend | 当没有未commit的更改时，显示最近的commit信息以更改，若有暂存区有更改则用此更改更新最新的commit
git revert SHA | 撤销SHA指定的commit，并添加一个新的commit
git reset --X SHA | X:a. mixed（默认）把commit放回工作区 b. soft把commit放回暂存区 c.把commit丢弃掉
git branch backup | 由于reset会删除掉当前分区commit因此可以考虑建立一个备份分支

### 祖先引用
- 对于一个分支，^表示第一个父亲 ^2表示第二个父亲
- ~N，表示当前分支上第n个父亲


