# xsel 
## chatgpt 
xsel is a command-line utility tool for manipulating the X11 primary selection buffer. The primary selection buffer is a part of the X Window System, and it stores any text highlighted or copied by users. The xsel command allows users to access and manipulate the contents of the primary selection buffer.

The xsel command can be used to perform a variety of operations, such as copying the contents of the primary selection buffer to the clipboard, appending text to the primary selection buffer, or clearing the contents of the buffer. Here are some examples of how to use the xsel command:

1. Copying the contents of the primary selection buffer to the clipboard:
   ```bash
   $ xsel --clipboard < file.txt
   ```
   Here, the contents of the file.txt file are copied to the primary selection buffer, and then the xsel command is used to copy those contents to the clipboard.

2. Appending text to the primary selection buffer:
   ```bash
   $ echo "new text" | xsel --append
   ```
   Here, the text "new text" is appended to the end of the primary selection buffer.

3. Clearing the primary selection buffer:
   ```bash
   $ xsel --clear
   ```
   This command clears the contents of the primary selection buffer.

In summary, the xsel command is a useful tool for manipulating the X11 primary selection buffer, allowing users to copy, append, and clear the contents of the buffer. 

## tldr 
 
> X11 selection and clipboard manipulation tool.
> More information: <https://manned.org/xsel>.

- Use a command's output as input of the clip[b]oard (equivalent to `Ctrl + C`):

`echo 123 | xsel -ib`

- Use the contents of a file as input of the clipboard:

`cat {{path/to/file}} | xsel -ib`

- Output the clipboard's contents into the terminal (equivalent to `Ctrl + V`):

`xsel -ob`

- Output the clipboard's contents into a file:

`xsel -ob > {{path/to/file}}`

- Clear the clipboard:

`xsel -cb`

- Output the X11 primary selection's contents into the terminal (equivalent to a mouse middle-click):

`xsel -op`
