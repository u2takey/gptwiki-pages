# git sync 
## chatgpt 
I'm sorry, but there is no "git sync" command in Git. 

However, there are a few Git commands that may be related to syncing changes between repositories:

1. git pull - this command fetches changes from a remote repository and merges them with the local repository.

2. git push - this command sends changes from the local repository to a remote repository.

3. git fetch - this command retrieves changes from a remote repository but does not merge them with the local repository.

It's worth noting that "syncing" in the context of Git usually refers to the process of updating your local repository with changes made in a remote repository, and vice versa. This can be done using a combination of the above commands depending on the specific use case. 

## tldr 
 
> Sync local branches with remote branches.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-sync>.

- Sync the current local branch with its remote branch:

`git sync`

- Sync the current local branch with the remote main branch:

`git sync origin main`

- Sync without cleaning untracked files:

`git sync -s {{remote_name}} {{branch_name}}`
