# git remote 
## chatgpt 
git remote是一个用于管理远程仓库的命令，它包含以下几个子命令：

1. git remote add <name> <url>：添加一个名为<name>，地址为<url>的远程仓库到本地仓库中。

2. git remote rename <old_name> <new_name>：将名为<old_name>的远程仓库重命名为<new_name>。

3. git remote remove <name>：从本地仓库中删除名为<name>的远程仓库。

4. git remote show <name>：显示名为<name>的远程仓库的信息，包括仓库地址、分支信息等。

5. git remote prune <name>：删除名为<name>的远程仓库中已经不存在的分支。

6. git remote update：将远程仓库中所有分支的最新状态更新到本地仓库中。 

总之，git remote命令用于管理本地仓库与远程仓库之间的关系，包括添加、重命名、删除、显示和更新等操作。 

## tldr 
 
> 管理跟踪的远程仓库（remotes）。
> 更多信息：<https://git-scm.com/docs/git-remote>.

- 列出已经存在的远程仓库，包括它们的名字和 URL：

`git remote -v`

- 查看某个远程仓库的信息：

`git remote show {{远程仓库名字}}`

- 添加远程仓库：

`git remote add {{远程仓库名字}} {{远程仓库 URL}}`

- 更改远程仓库地址链接（使用 `--add` 选项不会移除现有的 URL）：

`git remote set-url {{远程仓库名字}} {{新 URL}}`

- 移除远程仓库：

`git remote remove {{远程仓库名字}}`

- 重命名远程仓库：

`git remote rename {{旧名字}} {{新名字}}`
