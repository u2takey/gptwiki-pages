# git alias 
## chatgpt 
The 'git alias' command is used to create a customized shorthand of a Git command. It allows the user to create an alias for any Git command that they frequently use, but can't remember the exact syntax every time they use it. By creating an alias, the user can simply type the alias instead of the full command.

For example, if the user wants to create an alias for the 'git commit' command, they can type the following command:

```
git config --global alias.co commit
```

After running this command, the user can now use the shorthand 'git co' instead of 'git commit' to commit changes to their repository.

Similarly, the user can create aliases for other Git commands like 'git push', 'git pull', 'git status', etc.

The 'git alias' command is a powerful tool that can help the user save time and be more efficient while working with Git. However, it's important to use meaningful and easy to remember aliases to avoid confusion and mistakes. 

## tldr 
 
> Create shortcuts for Git commands.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-alias>.

- List all aliases:

`git alias`

- Create a new alias:

`git alias "{{name}}" "{{command}}"`

- Search for an existing alias:

`git alias ^{{name}}`
