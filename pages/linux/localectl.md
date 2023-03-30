# localectl 
## chatgpt 
`localectl` is a command-line tool that is used to query and modify the system's current keyboard layout and other localization settings.

When the `localectl` command is executed without any arguments, it displays the current system's localization settings, including the current keyboard layout, language, and other relevant settings. This includes the locale, the keyboard keymap, and the X11 keymap.

Some of the most common uses of the `localectl` command include:

- Displaying the current localization settings: `localectl`
- Changing the system's keyboard layout: `localectl set-keymap <keymap>`
- Setting the system's locale: `localectl set-locale <locale>`
- Displaying the list of available keymaps: `localectl list-keymaps`
- Displaying the list of available locales: `localectl list-locales`

Overall, the `localectl` command is an important tool for system administrators who need to maintain consistent localization settings across a variety of systems. 

## tldr 
 
> Control the system locale and keyboard layout settings.
> More information: <https://www.freedesktop.org/software/systemd/man/localectl.html>.

- Show the current settings of the system locale and keyboard mapping:

`localectl`

- List available locales:

`localectl list-locales`

- Set a system locale variable:

`localectl set-locale {{LANG}}={{en_US.UTF-8}}`

- List available keymaps:

`localectl list-keymaps`

- Set the system keyboard mapping for the console and X11:

`localectl set-keymap {{us}}`
