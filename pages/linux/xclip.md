# xclip 
## chatgpt 
xclip is a command-line tool that is used to copy or transfer text from one location to another within a Linux or Unix terminal environment. 

The basic syntax of the xclip command is: 

```xclip [options] [files]```

where options include different flags that enable the user to modify the behavior of the command.

Some commonly used options of the xclip command are:

- -selection: It is used to specify the type of selection to be used. For example, -selection clipboard specifies the clipboard selection, while -selection primary specifies the primary selection.

- -i: It is used to read data from standard input and copy it to the specified selection.

- -o: It is used to print the content of the specified selection to standard output.

- -l: It is used to specify the maximum size of the selection.

Example uses of the xclip command are:

- To copy the content of a file to the clipboard:

```cat file.txt | xclip -selection clipboard```

- To copy the output of a command to the clipboard:

```ls -l | xclip -selection clipboard```

- To paste the content of the clipboard into a file:

```xclip -selection clipboard -o > file.txt``` 

## tldr 
 
> X11 clipboard manipulation tool, similar to `xsel`.
> Handles the X primary and secondary selections, plus the system clipboard (`Ctrl + C`/`Ctrl + V`).
> More information: <https://manned.org/xclip>.

- Copy the output from a command to the X11 primary selection area (clipboard):

`echo 123 | xclip`

- Copy the output from a command to a given X11 selection area:

`echo 123 | xclip -selection {{primary|secondary|clipboard}}`

- Copy the output from a command to the system clipboard, using short notation:

`echo 123 | xclip -sel clip`

- Copy the contents of a file into the system clipboard:

`xclip -sel clip {{input_file.txt}}`

- Copy the contents of a PNG into the system clipboard (can be pasted in other programs correctly):

`xclip -sel clip -t image/png {{input_file.png}}`

- Copy the user input in the console into the system clipboard:

`xclip -i`

- Paste the contents of the X11 primary selection area to the console:

`xclip -o`

- Paste the contents of the system clipboard to the console:

`xclip -o -sel clip`
