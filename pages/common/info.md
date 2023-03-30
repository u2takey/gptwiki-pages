# info 
## chatgpt 
The "info" command is a command-line tool that provides detailed information about a specific topic or command. 

Syntax: 

```
info [OPTION]... [COMMAND | FILE]
```

The command can take two types of arguments:

1. COMMAND - If you provide a command as an argument, the tool will display information about that command. For example, ```info ls``` will display information about the "ls" command.

2. FILE - If you provide a file as an argument, the tool will display information about that file, including its contents, permissions, owner, and more. For example, ```info /etc/passwd``` will display information about the "passwd" file.

Some commonly used options with the "info" command are:

- "info --help": Displays a help message listing all available options and commands.
- "info --apropos=STRING": Searches for commands or topics that include the specified string.
- "info --index-search=STRING": Searches for commands or topics with a specific keyword in the info index.

Once you have launched the info command, you will be presented with a menu interface that you can navigate using the arrow keys, plus , minus (+, -) keys, and other options, to read the documentation and retrieve detailed information about the topics and commands used within the tool. 

## tldr 
 
> Reads documentation stored in the info format.
> More information: <https://en.wikipedia.org/wiki/Info_(Unix)>.

- Start reading top-level directory menu:

`info`

- Start reading at given menu item node from top-level directory:

`info {{menu_item}}`

- Start reading at second menu item within first menu item manual:

`info {{first_menu_item}} {{second_menu_item}}`
