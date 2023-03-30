# git rename-remote 
## chatgpt 
The "git rename-remote" command is used to rename a remote repository on the local machine. 

Syntax:
```
git rename-remote <old-name> <new-name>
```
Where "old-name" is the current name of the remote repository and "new-name" is the desired new name for the same remote repository.

Usage example:
Suppose you have a remote repository named "origin" and you want to rename it to "new-origin", the following command should be executed:
```
git rename-remote origin new-origin
``` 

Once executed, the remote repository will be renamed from "origin" to "new-origin" on the local machine. However, the change will not be reflected on the remote server until you use the "git push" command to push the changes to the remote repository. 

It is worth noting that to use the "git rename-remote" command, the user must have the necessary permissions to access the remote repository. 

## tldr 
 
> Change remote for pulling and pushing.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-rename-remote>.

- Change the upstream remote to origin:

`git rename-remote {{upstream}} {{origin}}`
