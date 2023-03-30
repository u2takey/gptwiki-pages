# git create-branch 
## chatgpt 
I'm sorry, but there is no "git create-branch" command in Git. The correct command to create a new branch in Git is "git branch".

The "git branch" command is used to create a new branch, list existing branches, or delete and rename branches. Here are the common syntax used with "git branch":

- To create a new branch: `git branch <branch-name>`
- To delete a branch: `git branch -d <branch-name>`
- To rename a branch: `git branch -m <new-branch-name>`
- To list all branches: `git branch`
- To switch to a branch: `git checkout <branch-name>`

For example, to create a new branch called "feature-branch", you would run the command:

```
git branch feature-branch
```

This will create a new branch based on the current branch you are on. You can then switch to this new branch by running the command:

```
git checkout feature-branch
```

Alternatively, you can create and switch to the new branch in one command by using:

```
git checkout -b feature-branch
``` 

## tldr 
 
> Create a Git branch in a repository.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-create-branch>.

- Create a local branch:

`git create-branch {{branch_name}}`

- Create a branch locally and on origin:

`git create-branch --remote {{branch_name}}`

- Create a branch locally and on upstream (through forks):

`git create-branch --remote upstream {{branch_name}}`
