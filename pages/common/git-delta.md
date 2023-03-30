# git delta 
## chatgpt 
There isn't a command "git delta" in Git. It might be a third-party tool that provides a visual representation of changes between commits, similar to "git diff". 

Here's a short explanation of "git diff" command:

"git diff" is a command in Git that shows changes between commits or working directory and the index or between the index and a tree. It's useful to understand what has been modified within a repository. 

The basic syntax of the command is:

```
git diff [options] [<commit>] [--] [<path>...]
```

- The first parameter "[options]" can be used to customize the output format and the scope of the diff. For example, the option "--color" adds color to the output, and the option "--name-only" shows only the names of the modified files.
- The second parameter "[<commit>]" specifies the commit to compare. If not specified, it compares the working directory and the index.
- The third parameter "[--]" is used to separate paths from options. It's optional.
- The last parameter "[<path>...]" specifies the path to a file or directory to compare. If not specified, it shows all the modified files.

Example usages:

- Show the changes in the last commit:
```
git diff HEAD^ HEAD
```

- Show the changes between two branches:
```
git diff branch1..branch2
```

- Show the changes in a specific file:
```
git diff file.txt
```

- Show the names of the modified files:
```
git diff --name-only
``` 

## tldr 
 
> List files that differ from another branch.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-delta>.

- List files from the current checked out branch that differ from the `main` branch:

`git delta {{main}}`

- List files from a specific branch that differ from another specific branch:

`git delta {{branch_1}} {{branch_2}}`
