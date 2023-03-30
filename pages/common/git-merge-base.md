# git merge-base 
## chatgpt 
The `git merge-base` command is used to find the common ancestor of two or more branches, which can help in identifying the changes that have been made to these branches since they diverged. 

To use the `git merge-base` command, you need to specify the names of the branches whose common ancestor you want to find. For example, to find the common ancestor of the `master` and `feature` branches, you would run the following command:

```
git merge-base master feature
```

The command will output a commit SHA which represents the common ancestor of the two branches. 

If you need to find the common ancestor of more than two branches, you can include multiple branch names as arguments:

```
git merge-base branch1 branch2 branch3
```

The `git merge-base` command can be useful in various scenarios, such as before performing a merge or rebase operation, or when you need to identify the changes that have been made to a branch since it was forked from another branch. 

## tldr 
 
> Find a common ancestor of two commits.
> More information: <https://git-scm.com/docs/git-merge-base>.

- Print the best common ancestor of two commits:

`git merge-base {{commit_1}} {{commit_2}}`

- Output all best common ancestors of two commits:

`git merge-base --all {{commit_1}} {{commit_2}}`

- Check if a commit is an ancestor of a specific commit:

`git merge-base --is-ancestor {{ancestor_commit}} {{commit}}`
