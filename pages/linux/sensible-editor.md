# sensible-editor 
## chatgpt 
The `sensible-editor` command is a Debian/Ubuntu Linux utility that uses the user's preferred editor to open and edit a file. 

When a user types in the `sensible-editor` command on the terminal, it reads the user's environment variables to determine the preferred editor. It looks for the `EDITOR` and `VISUAL` environment variables, which contain the path to the user's preferred editor. 

If the `EDITOR` variable is set, it uses that editor. If it is not, it checks the `VISUAL` variable. If neither variable is set, it falls back to a default editor defined by the system. 

Once it determines the preferred editor, it opens a new instance of that editor and waits for the user to edit a file. The command will not execute until the editor is closed, and then it will output any changes made to the file. 

This command is helpful when a user needs to edit a file and isn't sure which editor to use or wants to use the preferred editor that is set in their environment variables. 

## tldr 
 
> Open the default editor.
> More information: <https://manned.org/sensible-editor>.

- Open a file in the default editor:

`sensible-editor {{path/to/file}}`

- Open a file in the default editor, with the cursor at the end of the file:

`sensible-editor + {{path/to/file}}`

- Open a file in the default editor, with the cursor at the beginning of line 10:

`sensible-editor +10 {{path/to/file}}`

- Open 3 files in vertically split editor windows at the same time:

`sensible-editor -O3 {{file_1}} {{file_2}} {{file_3}}`
