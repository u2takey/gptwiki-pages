# bashmarks 
## chatgpt 
Bashmarks is not actually a command, but a script that can be added to your Bash shell to use bookmarks to quickly navigate to your frequently-used directories. 

When you add Bashmarks to your Bash shell, you can create new bookmarks using the `bookmark` command, which takes one argument – the name of the bookmark you want to create. For example, if you want to create a bookmark for your home directory, you could use the command `bookmark home`.

Once you have created a bookmark, you can use the `cd` command with the bookmark name to quickly navigate to that directory. For example, if you created a bookmark called "projects" for your projects folder, you could use the command `cdp projects` to go to that folder.

You can also use the `lsp` command to list all your bookmarks, `delbookmark` to delete a bookmark, and `clearexpired` to clear any expired bookmarks.

Overall, Bashmarks is a convenient tool that can help streamline your workflow by allowing you to quickly navigate to frequently-used directories with just a few keystrokes. 

## tldr 
 
> Save and jump to commonly used directories using 1 character commands.
> More information: <https://github.com/huyng/bashmarks>.

- List available bookmarks:

`l`

- Save the current directory as "bookmark_name":

`s {{bookmark_name}}`

- Go to a bookmarked directory:

`g {{bookmark_name}}`

- Print a bookmarked directory's contents:

`p {{bookmark_name}}`

- Delete a bookmark:

`d {{bookmark_name}}`
