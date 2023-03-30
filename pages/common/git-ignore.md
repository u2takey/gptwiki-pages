# git ignore 
## chatgpt 
The `git ignore` command is used to exclude files or directories from being tracked by Git. This command adds the specified file or directory to a list of ignored files and Git will never stage, commit or push changes to any file that matches patterns in the specified file.

Typically, this command is used when you have files that should not be committed to a repository, such as compiled code, configuration files, or temporary files. This can help keep the repository clean and prevent conflicts.

To use the `git ignore` command, you simply need to specify the file or directory you want to ignore. For example, to ignore a directory called `build`, you would run:

```
git ignore build
```

You can also create a file called `.gitignore` in the root directory of your repository and add patterns for files or directories you want to ignore. This file should be committed to the repository.

Examples of patterns that can be added to `.gitignore` include:

- `*.log`:  Ignores all files with the extension `log`
- `build/`: Ignores the entire directory `build`
- `config.json`: Ignores a specific file named `config.json`

Once files are ignored, they will no longer show up in the list of untracked files when running `git status`. 

## tldr 
 
> Show/update `.gitignore` files.
> Part of `git-extras`. See also `git ignore-io`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-ignore>.

- Show the content of all global and local `.gitignore` files:

`git ignore`

- Ignore file(s) privately, updating `.git/info/exclude` file:

`git ignore {{file_pattern}} --private`

- Ignore file(s) locally, updating local `.gitignore` file:

`git ignore {{file_pattern}}`

- Ignore file(s) globally, updating global `.gitignore` file:

`git ignore {{file_pattern}} --global`
