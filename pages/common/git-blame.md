# git blame 
## chatgpt 
The `git blame` command is used to display the author and the last modification made to each line of a file. The command is often used to track changes made to a file over time and to see who made which changes. 

When you run `git blame`, it will print the contents of a file along with each line's commit hash, author name, and the date and time the line was last modified. The command also displays a line-by-line annotation of changes made to a file, along with the author of each change.

For example, let's say you want to know who made changes to a file named 'file.txt'. You can run the following command:

```
git blame file.txt
```

This will display the file contents along with the commit hash, author name, and the date and time of the last modification made to each line of the file. You can use this information to determine who made specific changes and when those changes were made. 

Overall, `git blame` is a useful command for tracking changes made to a file and understanding the history of modifications made to it. 

## tldr 
 
> Show commit hash and last author on each line of a file.
> More information: <https://git-scm.com/docs/git-blame>.

- Print file with author name and commit hash on each line:

`git blame {{path/to/file}}`

- Print file with author email and commit hash on each line:

`git blame -e {{path/to/file}}`

- Print file with author name and commit hash on each line at a specific commit:

`git blame {{commit}} {{path/to/file}}`

- Print file with author name and commit hash on each line before a specific commit:

`git blame {{commit}}~ {{path/to/file}}`
