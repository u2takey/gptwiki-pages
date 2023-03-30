# view 
## chatgpt 
The view command is a command line utility that is used to display the contents of a file on the terminal screen without modifying the original file. Here are some details about the view command:

Syntax:
view [options] [filename]

Options:
- [+]n: Starts the view command at line n.
- [-]n: Starts the view command n lines from the end of the file.
- /pattern: Searches the file for pattern and goes to the first occurrence of pattern.
- ?pattern: Searches the file for pattern and goes to the last occurrence of pattern.
- q: Quits the view command.

Usage:

To display the contents of a file on the terminal screen, simply type 'view' followed by the name of the file you want to open. For example:

view myFile.txt 

This will display the contents of myFile.txt on the terminal screen. 

You can also use the +n and -n options to start the view command from a specific line number. For example:

view +10 myFile.txt 

This will start the view command at line 10 of myFile.txt. 

If you want to search for a specific pattern in the file, you can use the /pattern or ?pattern option. For example:

view /hello myFile.txt 

This will search for the first occurrence of 'hello' in myFile.txt and display it on the terminal screen. 

Finally, to quit the view command, simply type 'q' on the terminal screen. 

## tldr 
 
> A read-only version of `vim`.
> This is equivalent to `vim -R`.
> More information: <https://www.vim.org>.

- Open a file:

`view {{path/to/file}}`
