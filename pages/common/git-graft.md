# git graft 
## chatgpt 
The `git graft` command is used in Git to create a new commit that connects two different lineages of a repository's history as if they were always part of the same branch. It is also used to combine multiple branches that have diverged across different versions.

The command works by editing the git graft file, `.git/info/grafts` to specify parent commit(s) to connect two branches. This temporary connection will persist until the operation is deliberately removed.

The syntax of the git graft command is:

```
git graft <commit> [<parent>…]
```

where `commit` is the commit object that will have its parent(s) changed and `parent` is the SHA-1 hash or branch name that will be added as its new parent.

After updating grafted commits, `git filter-branch` can be used to apply these changes permanently. However, it's important to note that `git graft` is an old and rarely used command in modern Git workflows. 
It’s better to use `git rebase` or `git merge` to join different branches in most cases. 

## tldr 
 
> Merge commits from a specific branch into another branch and delete the source branch.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-graft>.

- Merge all commits not present on the target branch from the source branch to target branch, and delete the source branch:

`git graft {{source_branch}} {{target_branch}}`
