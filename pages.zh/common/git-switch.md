# git switch 
## chatgpt 
git switch 命令用于切换分支或恢复工作区文件。其用法如下：

```
git switch [-c] <分支名>               # 创建并切换到新分支
git switch [-f|--force] [<分支名>]      # 强制切换到分支并丢弃本地修改
git switch [--detach] [<提交号>]       # 切换到某次提交的状态，丢失分支信息
git switch [-]                            # 在最近使用的两个分支之间切换
git switch [-n|--no-checkout] <文件名>  # 不切换分支，仅更新指定文件。  
```

具体解释如下：

1. `git switch -c <分支名>`：创建并切换到新分支。
   
   这个命令相当于执行了 `git branch <分支名>` 和 `git checkout <分支名>` 两个命令。如果当前分支有未提交的更改，需要先提交或者 stash 手头的修改。举个例子，创建并切换到一个名为 `feature-1` 的新分支，可以使用命令：`git switch -c feature-1`

2. `git switch <分支名>`：切换到指定分支。
   
   这个命令和 `git checkout <分支名>` 等价，用于切换到已存在的分支。如果当前分支有未提交的更改，需要先提交或者 stash 手头的修改。例如，如果想要切换到 `develop` 分支，可以运行：`git switch develop`

3. `git switch -f|--force [<分支名>]`：强制切换到分支并丢弃本地修改。
   
   如果本地修改和分支内容冲突，该命令可以强制切换到指定分支，并丢弃本地修改。如果没有指定分支名，则表示强制切换到当前所在的分支。例如，执行以下命令可以强制切换到 `main` 分支，并丢弃本地修改：`git switch -f main`

4. `git switch --detach [<提交号>]`：切换到某次提交的状态，丢失分支信息。
   
   该命令可以将 HEAD 指针移动到指定提交，并在“分离 HEAD”状态下工作。这意味着 HEAD 不再位于任何分支上，且本地修改将不会被保存，除非将其 stash 起来。如果没有指定提交号，则默认切换到最新提交。例如，执行以下命令可以将 HEAD 指针移动到最新提交，并进入“分离 HEAD”状态下工作：`git switch --detach`

5. `git switch -`：在最近使用的两个分支之间切换。
   
   该命令可以在最近使用的两个分支之间切换。在切换分支之前，该命令会将当前分支的修改 stash 起来，以便切换到另一分支。例如，如果要在 `develop` 分支和 `feature-1` 分支之间来回切换，可以运行：`git switch -`

7. `git switch [-n|--no-checkout] <文件名>`：不切换分支，仅更新指定文件。
   
   该命令可以在不切换分支的情况下，更新指定文件。这在需要在本地修改文件，并将其保存为某个提交的情况下非常有用。如果使用 `-n` 或 `--no-checkout` 选项，则不会切换分支，而是将指定文件的内容更新为给定提交的内容。例如，要更新文件 `README.md` 的内容为 `deadbeef` 提交的内容，可以使用如下命令：`git switch -n deadbeef -- README.md` 

## tldr 
 
> 切换 Git 分支。要求 Git 版本在 2.23 以上。
> 另请参阅 `git checkout`。
> 更多信息：<https://git-scm.com/docs/git-switch>.

- 切换到一个已有的分支：

`git switch {{分支名字}}`

- 创建并切换到一个新分支：

`git switch --create {{分支名字}}`

- 创建并切换到基于某个提交的新分支：

`git switch --create {{分支名字}} {{指定提交}}`

- 切换到之前的分支：

`git switch -`

- 切换到一个分支，并更新所有匹配的子模块：

`git switch --recurse-submodules {{分支名字}}`

- 切换到一个分支，并和当前分支以及暂未提交的修改进行三方合并：

`git switch --merge {{分支名字}}`
