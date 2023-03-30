# git clear-soft 
## chatgpt 
I'm sorry, but there is no "git clear-soft" command in Git. It might be possible that you are referring to the "git clean" command.

Git Clean: 

The "git clean" command is used to remove untracked files from the working directory. Untracked files are files that are not managed by Git. These files can be created by the user or by some other process outside Git's control. Removing these files can help in keeping the working directory clean.

The syntax for the git clean command is:

```git clean [options]```

The commonly used options are:

- -n or --dry-run: This option is used to preview the files that will be deleted without actually deleting them.
- -f or --force: This option is used to forcefully delete files from the working directory.

For example, to delete all untracked files from the working directory, you can run the following command:

```git clean -f```

This will remove all files that are not tracked by Git. It is important to use this command with caution as it can delete files permanently. 

## tldr 
 
> Clear a Git working directory as if it was freshly cloned with the current branch excluding files in `.gitignore`.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-clear-soft>.

- Reset all tracked files and delete all untracked files:

`git clear-soft`
