# git branch 
## chatgpt 
The command "git branch" is used to list, create or delete branches in a Git repository. Here's a detailed explanation of what each option does:

1. "git branch": This option lists all the local branches that exist in the current Git repository.

2. "git branch -r": This option lists all the remote tracking branches available in the repository.

3. "git branch -a": This option shows a list of both local and remote branches available in the repository.

4. "git branch [branch_name]": This option is used to create a new branch with the specified name.

5. "git branch -d [branch_name]": This option is used to delete a branch with the specified name.

6. "git branch -D [branch_name]": This option is used to forcefully delete the specified branch, even if it has not been merged into the main branch.

Overall, the "git branch" command is a powerful tool for managing the branches in a Git repository. 

## tldr 
 
> Main Git command for working with branches.
> More information: <https://git-scm.com/docs/git-branch>.

- List all branches (local and remote; the current branch is highlighted by `*`):

`git branch --all`

- List which branches include a specific Git commit in their history:

`git branch --all --contains {{commit_hash}}`

- Show the name of the current branch:

`git branch --show-current`

- Create new branch based on the current commit:

`git branch {{branch_name}}`

- Create new branch based on a specific commit:

`git branch {{branch_name}} {{commit_hash}}`

- Rename a branch (must not have it checked out to do this):

`git branch -m {{old_branch_name}} {{new_branch_name}}`

- Delete a local branch (must not have it checked out to do this):

`git branch -d {{branch_name}}`

- Delete a remote branch:

`git push {{remote_name}} --delete {{remote_branch_name}}`
