# git force-clone 
## chatgpt 
There is no git command called "force-clone". The correct command to clone a repository in Git is "git clone". 

"git clone" is a command used to create a copy of a remote repository in your local machine. The command downloads the entire repository from the remote server and creates a local copy of it. The syntax of the command is as follows:

```
git clone <repository-url>
```

If you want to download a specific branch of the repository, you can specify it in the command as follows:

```
git clone -b <branch-name> <repository-url>
```

The "force" option is not applicable to the "git clone" command. Overall, there is no such command as "git force-clone". 

## tldr 
 
> Provides the basic functionality of `git clone`, but if the destination git repository already exists it will force-reset it to resemble a clone of the remote.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-force-clone>.

- Clone a Git repository into a new directory:

`git force-clone {{remote_repository_location}} {{path/to/directory}}`

- Clone a Git repository into a new directory, checking out an specific branch:

`git force-clone -b {{branch_name}} {{remote_repository_location}} {{path/to/directory}}`

- Clone a Git repository into an existing directory of a Git repository, performing a force-reset to resemble it to the remote and checking out an specific branch:

`git force-clone -b {{branch_name}} {{remote_repository_location}} {{path/to/directory}}`
