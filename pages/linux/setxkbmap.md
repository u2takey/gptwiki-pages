# setxkbmap 
## chatgpt 
The `setxkbmap` command in Linux is used to set the keyboard layout for the current session or permanently. It is used to change the attributes of the keyboard mapping in X. 

The `setxkbmap` command allows the user to set the keyboard map that is used by X. The command takes a number of arguments which specify various aspects of the keyboard map, such as the layout of keys, the language that is being typed, and any special keys that are included.

The most basic form of the `setxkbmap` command is as follows:

     setxkbmap <options>

The `<options>` can include which layout to use, which language to use, and any special options such as enabling the Caps Lock key as a Control key.

Some common options for the `setxkbmap` command include:

- `-model`: specifies the keyboard model to use.

- `-layout`: specifies the keyboard layout to use.

- `-variant`: specifies the variant of the keyboard layout.

- `-option`: specifies additional options to be used with the keyboard map.

For example, the command `setxkbmap -layout us -variant intl` would set the keyboard to use the US layout with the international variant.

The `setxkbmap` command allows the user to customize their keyboard settings in Linux, making it easier to type in different languages or with special requirements. 

## tldr 
 
> Set the keyboard using the X Keyboard Extension.
> More information: <https://manned.org/setxkbmap>.

- Set the keyboard in French AZERTY:

`setxkbmap {{fr}}`

- Set multiple keyboard layouts, their variants and switching option:

`setxkbmap -layout {{us,de}} -variant {{,qwerty}} -option {{'grp:alt_caps_toggle'}}`

- Get help:

`setxkbmap -help`

- List all layouts:

`localectl list-x11-keymap-layouts`

- List variants for the layout:

`localectl list-x11-keymap-variants {{de}}`

- List available switching options:

`localectl list-x11-keymap-options | grep grp:`
