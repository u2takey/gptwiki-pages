# git rename-branch 
## chatgpt 
git rename-branch命令用于将分支重命名。

命令的语法如下：

```
git rename-branch <旧分支名称> <新分支名称>
```

执行此命令后，Git会将本地仓库中的旧分支名称修改为新分支名称，同时也会将远程仓库中的分支名称修改为新分支名称。

需要注意的是，如果当前分支是重命名前的分支，则需要切换到其他分支或创建新分支，才能完成重命名操作。

另外，如果远程仓库已经将旧分支名称删除，则需要使用如下命令将重命名后的分支推送到远程仓库：

```
git push origin :<旧分支名称> <新分支名称>
```

这条命令会删除远程仓库中的旧分支名称，并将新的分支推送到远程仓库。 

## tldr 
 
> 重新命名一个 Git 分支。
> 属于 `git-extras` 的一部分。
> 更多信息：<https://github.com/tj/git-extras/blob/master/Commands.md#git-rename-branch>.

- 重新命名你目前所在的分支：

`git rename-branch {{新的分支名称}}`

- 重新命名一个特定的分支：

`git rename-branch {{旧的分支名称}} {{新的分支名称}}`
