# wsl-open 
## chatgpt 
The "wsl-open" command is a command used in Windows Subsystem for Linux (WSL) environment to open a file or URL in the default Windows application associated with that type of file or URL. 

This command is similar to the Linux "xdg-open" command which is used to open a file or URL in the default Linux application associated with that type of file or URL. 

The "wsl-open" command is often used in command-line scripts or programs in WSL to open files or URLs in the default Windows application. For example, if you want to open a PDF file in the default Windows PDF viewer, you can use the command "wsl-open myfile.pdf" and it will automatically open the file in the default Windows PDF viewer. Similarly, if you want to open a website in the default Windows web browser, you can use the command "wsl-open https://www.google.com" and it will automatically open the website in the default Windows web browser. 

In summary, the "wsl-open" command is a useful command in the WSL environment which allows opening files or URLs in the default Windows application quickly and easily. 

## tldr 
 
> Open a file or URL from within Windows Subsystem for Linux in the user's default Windows GUI application.
> More information: <https://gitlab.com/4U6U57/wsl-open>.

- Open the current directory in Windows Explorer:

`wsl-open {{.}}`

- Open a URL in the user's default web browser in Windows:

`wsl-open {{https://example.com}}`

- Open a specific file in the user's default application in Windows:

`wsl-open {{path\to\file}}`

- Set `wsl-open` as the shell's web browser (open links with `wsl-open`):

`wsl-open -w`

- Display help:

`wsl-open -h`
