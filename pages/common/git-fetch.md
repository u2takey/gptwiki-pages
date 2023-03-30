# git fetch 
## chatgpt 
The `git fetch` command is used in Git version control system to download and update remote branches, tags, and their respective commit history from a remote repository to the local repository. It is often used to synchronize a local repository with a remote repository.

When you run `git fetch`, Git will contact the remote repository and download any changes made since the last time you fetched or pulled. It will not integrate any changes into your local branch, but it will update the remote tracking branch so that you know about any changes that were made on the remote repository. 

It updates the `origin/master` (or any other remote branch) to the latest version on the remote repository but does not merge the changes into the current branch. You still need to run `git merge` or `git pull` to update the local branch with the latest changes from the remote repository.

In summary, `git fetch` is used to update your local repository's knowledge of the history of a remote repository without causing any changes in your local working directory. It is safe to use and can be run as often as required without the risk of losing data or causing conflicts. 

## tldr 
 
> Download objects and refs from a remote repository.
> More information: <https://git-scm.com/docs/git-fetch>.

- Fetch the latest changes from the default remote upstream repository (if set):

`git fetch`

- Fetch new branches from a specific remote upstream repository:

`git fetch {{remote_name}}`

- Fetch the latest changes from all remote upstream repositories:

`git fetch --all`

- Also fetch tags from the remote upstream repository:

`git fetch --tags`

- Delete local references to remote branches that have been deleted upstream:

`git fetch --prune`
