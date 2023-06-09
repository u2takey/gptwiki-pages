# git rebase 
## chatgpt 
git rebase命令用于将一个分支的修改重放在另一个分支上，其基本作用是将源分支的提交应用于目标分支。

具体来讲，git rebase操作会将当前分支(A分支)的基底变为目标分支(B分支)上指定的提交，然后将当前分支中的所有提交都暂存为补丁(patch)格式，接着将当前分支中的所有提交移动到目标分支(B分支)之上，最后一个个应用这些补丁。

使用git rebase可以将分支合并历史简单化，不像git merge那样会创建新的合并提交，而是通过将源分支的修改应用到目标分支上来达到合并的效果。

命令语法：

```
git rebase <base>
```

参数说明：

- `<base>`为目标分支，即希望将修改应用到哪个分支上。

常用选项：

- `--interactive`：允许交互式的变基。

注意事项：

- rebase操作会改变分支历史，如果公共仓库有多人协作时，应当慎用。

- 如果在变基的过程中出现了冲突，需要手动解决并进行提交，这可能会增加一些复杂性。

- 由于rebase会修改历史，所以在合并分支后使用git push推送分支时可能会遇到“因为ref被更新而拒绝”的错误。此时需要使用git push --force进行强制推送。 

## tldr 
 
> 将 commits 从一个分支合并到另一个分支上。
> 常用于跨分支的 commits 合并，在被合并分支的最头部构建新的 `commit`，表示合并完成。
> 更多信息：<https://git-scm.com/docs/git-rebase>.

- 在另一个分支的头节点合并当前分支：

`git rebase {{目标分支}}`

- 启动交互式的合并任务，允许对提交的内容进行重新排序、省略、合并或修改：

`git rebase -i {{目标分支或 commit 的 hash}}`

- 处理完冲突文件后，继续执行合并任务：

`git rebase --continue`

- 跳过冲突文件，继续执行合并任务：

`git rebase --skip`

- 终止正在执行中的合并任务（例如：对于正处于解决冲突中的任务，将其打断，恢复到合并前的状态）：

`git rebase --abort`

- 将分支的部分 commits 生成新的 `commit`，移动到新分支的头节点：

`git rebase --onto {{目标分支}} {{当前分支}}`

- 启动交互式的合并任务，对最近提交的 5 个 commits 进行重新排序、省略、合并或修改：

`git rebase -i {{HEAD~5}}`

- 以当前分支优先的策略，自动处理分支间的冲突，执行合并：

`git rebase -X theirs {{分支名称}}`
