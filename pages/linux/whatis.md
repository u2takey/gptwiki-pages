# whatis 
## chatgpt 
The "whatis" command is a Linux utility that displays a short one-line description of a command or function in the terminal. It is a quick way to get a brief overview of what a command does and its usage. 

The syntax for the command is simple: 

`whatis [command or function name]`

For example, to see a brief description of the "ls" command, you can type:

`whatis ls`

The output will be:

`ls   (1)  - list directory contents`

The "1" in parentheses indicates the section of the manual where you can find more information about the command, in this case, section 1 which contains general commands. 

The "whatis" command is useful for quickly checking the purpose of a command or function, especially if you're new to the command line environment or trying to learn a new tool. However, it only displays one-line descriptions, so if you need more detailed information, you'll need to consult the manual pages. 

## tldr 
 
> Display one-line descriptions from manual pages.
> More information: <https://manned.org/whatis>.

- Display a description from a man page:

`whatis {{command}}`

- Don't cut the description off at the end of the line:

`whatis --long {{command}}`

- Display descriptions for all commands matching a glob:

`whatis --wildcard {{net*}}`

- Search man page descriptions with a regular expression:

`whatis --regex '{{wish[0-9]\.[0-9]}}'`

- Display descriptions of a specific language (requires `manpage-{{locale}}` package):

`whatis --locale={{en}} {{command}}`
