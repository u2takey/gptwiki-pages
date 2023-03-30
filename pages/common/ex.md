# ex 
## chatgpt 
"ex" is a command-line text editor that is primarily used in Unix-based operating systems such as Linux and macOS. It is the predecessor to the more popular vi and vim editors.

When you run the "ex" command, you will have access to a command-line interface that allows you to open, edit, and save text files. The basic syntax for using the "ex" command is as follows:

ex [option] [file]

Here, the "option" parameter is optional and can be used to specify various options for the "ex" editor. The "file" parameter is the name of the file you want to edit.

Once you have launched the "ex" editor, you can use various commands to navigate and modify your text file. These commands are typically entered in "command mode", which is the default mode the editor starts in.

Some commonly used "ex" commands include:

- :w → Save changes to the file
- :q → Quit the editor
- :q! → Quit the editor without saving changes
- :wq → Save changes and quit the editor
- :set number → Display line numbers in the editor
- :/<search pattern> → Search for a specific pattern in the file
- :s/<old>/<new>/g → Replace all occurrences of "old" with "new" in the current line
- :%s/<old>/<new>/g → Replace all occurrences of "old" with "new" in the entire file

Overall, the "ex" command provides a simple and lightweight text editor that is ideal for working with text files in a Unix-based environment. 

## tldr 
 
> Command-line text editor.
> See also: `vim`.
> More information: <https://www.vim.org>.

- Open a file:

`ex {{path/to/file}}`

- Save and Quit:

`wq<Enter>`

- Undo the last operation:

`undo<Enter>`

- Search for a pattern in the file:

`/{{search_pattern}}<Enter>`

- Perform a regular expression substitution in the whole file:

`%s/{{regular_expression}}/{{replacement}}/g<Enter>`

- Insert text:

`i<Enter>{{text}}<C-c>`

- Switch to Vim:

`visual<Enter>`
