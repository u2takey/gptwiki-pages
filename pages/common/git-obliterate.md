# git obliterate 
## chatgpt 
I'm sorry, but there is no `git obliterate` command in Git. Therefore, I cannot provide a detailed explanation of this command. It is possible that you may have mistaken it for some other command or that it is a custom command created by a specific Git installation or plugin. In general, Git provides several commands for managing and manipulating the commit history, repository contents, and branches, such as `git commit`, `git checkout`, `git merge`, `git reset`, `git rebase`, etc. You can refer to the Git documentation or run `git --help` or `git <command> --help` to learn more about each command and its usage. 

## tldr 
 
> Delete specific files and erase their history from a Git repository.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-obliterate>.

- Erase the existence of specific files:

`git obliterate {{file_1 file_2 ...}}`

- Erase the existence of specific files between 2 commits:

`git obliterate {{file_1 file_2 ...}} -- {{commit_hash_1}}..{{commit_hash_2}}`
