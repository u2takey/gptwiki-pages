# nano 
## chatgpt 
Nano is a text editor in Linux and macOS operating systems. It allows users to create and edit text files using the command line rather than a graphical user interface (GUI). To launch Nano, one can simply type "nano" followed by the name of the file they wish to edit.

For example, to create a new text file called "mytextfile.txt" using Nano, one can enter the following command:

```nano mytextfile.txt```

This will open up the text editor with a blank file called "mytextfile.txt" ready to be edited. Within Nano, users can use various commands to manipulate the text on the screen.

Some common commands in Nano include: 

- **Ctrl + G**: help menu for all available commands
- **Ctrl + O**: save the file and exit Nano
- **Ctrl + X**: exit Nano without saving
- **Ctrl + K**: cut a highlighted block of text
- **Ctrl + U**: paste a cut block of text

Overall, Nano is a simple but powerful text editor that can be used to create and edit files in a command line environment. 

## tldr 
 
> Command-line text editor. An enhanced `Pico` clone.
> More information: <https://nano-editor.org>.

- Start the editor:

`nano`

- Start the editor without using configuration files:

`nano --ignorercfiles`

- Open specific files, moving to the next file when closing the previous one:

`nano {{path/to/file1 path/to/file2 ...}}`

- Open a file and position the cursor at a specific line and column:

`nano +{{line}},{{column}} {{path/to/file}}`

- Open a file and enable soft wrapping:

`nano --softwrap {{path/to/file}}`

- Open a file and indent new lines to the previous line's indentation:

`nano --autoindent {{path/to/file}}`

- Open a file and create a backup file (`path/to/file~`) on save:

`nano --backup {{path/to/file}}`
