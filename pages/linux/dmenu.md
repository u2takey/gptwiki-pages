# dmenu 
## chatgpt 
dmenu is a dynamic menu or program launcher for X Window System, typically used in Linux or UNIX operating systems. 

When executed, dmenu displays a list of items, usually programs or commands, from which the user can choose by typing the (case-insensitive) name of the item, and then pressing Enter to execute the corresponding program or command. The list of items can be generated manually or automatically by a script. 

The syntax for using dmenu is:

```
dmenu [options] [arguments]
```

Some of the most commonly used options are:

- -b: Show dmenu at the bottom of the screen
- -l: Lines to display (default: 10)
- -i: Case-insensitive matching
- -fn: Font to use
- -nf: Normal foreground color
- -nb: Normal background color
- -sf: Selected foreground color
- -sb: Selected background color

Examples:

1. Launching a program using dmenu:

```
dmenu_run
```

This will display a list of available programs in the $PATH environment variable. Typing the name of a program and pressing Enter will launch it.

2. Launching a program using a file list:

```
find $HOME -type f | dmenu | xargs -rxd '\n' sh -c 'exec "$@"' sh
```

This will display a list of all files in the user's home directory. Typing the name of a file and pressing Enter will execute it.

3. Launching a command with arguments:

```
cat $HOME/.bash_history | sort | uniq | dmenu -p "History:" | xargs -r -I % sh -c "echo % | xclip -i"
```

This will display a list of unique commands from the user's Bash command history. Typing the name of a command and pressing Enter will copy it to the clipboard using the xclip command. 

## tldr 
 
> Dynamic menu.
> Creates a menu from a text input with each item on a new line.
> More information: <https://manned.org/dmenu>.

- Display a menu of the output of the `ls` command:

`{{ls}} | dmenu`

- Display a menu with custom items separated by a new line (`\n`):

`echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu`

- Let the user choose between multiple items and save the selected one to a file:

`echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu > {{color.txt}}`

- Launch dmenu on a specific monitor:

`ls | dmenu -m {{1}}`

- Display dmenu at the bottom of the screen:

`ls | dmenu -b`
