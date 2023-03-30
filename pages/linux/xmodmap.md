# xmodmap 
## chatgpt 
xmodmap is a command used in Linux and Unix operating systems to modify the key mappings of a keyboard. It is used to remap certain keys or to create new key bindings.

The xmodmap utility allows users to redefine the keyboard keys by changing the way the system interprets the input from the keyboard. This is achieved by running the xmodmap command followed by a set of options that define the desired key mappings.

Some common uses of the xmodmap command include swapping the keys on a keyboard (such as swapping the Caps Lock and Control keys), mapping non-standard keys (such as multimedia keys), and defining custom key bindings (such as launching a specific application with a single key press).

To use xmodmap, users need to create a file with the key mappings they want to use and then run the "xmodmap filename" command to load the file. The file should contain a list of keys and the action or key combination that should be associated with each key.

Overall, xmodmap is a powerful command that allows users to customize their keyboard layout to suit their preferences and workflow. 

## tldr 
 
> Utility for modifying keymaps and pointer button mappings in X.
> More information: <https://manned.org/xmodmap>.

- Swap left-click and right-click on the pointer:

`xmodmap -e 'pointer = 3 2 1'`

- Reassign a key on the keyboard to another key:

`xmodmap -e 'keycode {{keycode}} = {{keyname}}'`

- Disable a key on the keyboard:

`xmodmap -e 'keycode {{keycode}} ='`

- Execute all xmodmap expressions in the specified file:

`xmodmap {{path/to/file}}`
