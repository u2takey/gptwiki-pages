# git check-ignore 
## chatgpt 
The `git check-ignore` command is used to check whether a specific path or file is ignored by Git based on the rules specified in the `.gitignore` file. 

The command takes one or more file/directory paths as arguments and verifies whether each of them is ignored by Git. If a path is being ignored, the output will display the corresponding `.gitignore` rule that is responsible for ignoring it.

Syntax:
```
git check-ignore <path> [<path> ...]
```

Example:
Suppose we have a `.gitignore` file that includes the following rules:
```
# ignore everything inside build/ directory
build/*

# ignore log files
*.log

# ignore a specific file
config.yml
```

If we want to check whether a file named `config.yml` is being ignored by Git or not, we can use the following command:
```
$ git check-ignore config.yml
.gitignore:4:config.yml
```
In this example, the output shows that the `.gitignore` rule specified in line 4 is responsible for ignoring the `config.yml` file.

Similarly, we can check whether multiple files/directories are being ignored:
```
$ git check-ignore build/script.sh .gitignore
.gitignore:2:build/*
.gitignore:6:.gitignore
```
This output indicates that the `.gitignore` rule specified in line 2 is responsible for ignoring the `build/script.sh` file, whereas the rule in line 6 has caused the `.gitignore` file itself to be ignored. 

## tldr 
 
> Analyze and debug Git ignore / exclude (".gitignore") files.
> More information: <https://git-scm.com/docs/git-check-ignore>.

- Check whether a file or directory is ignored:

`git check-ignore {{path/to/file_or_directory}}`

- Check whether multiple files or directories are ignored:

`git check-ignore {{path/to/file}} {{path/to/directory}}`

- Use pathnames, one per line, from `stdin`:

`git check-ignore --stdin < {{path/to/file_list}}`

- Do not check the index (used to debug why paths were tracked and not ignored):

`git check-ignore --no-index {{path/to/files_or_directories}}`

- Include details about the matching pattern for each path:

`git check-ignore --verbose {{path/to/files_or_directories}}`
