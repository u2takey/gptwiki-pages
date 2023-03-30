# rofi 
## chatgpt 
Rofi is a powerful and highly customizable application launcher that can be used in place of other launchers like dmenu. It offers a wide range of features including:

- Search functionality: You can easily search for applications, files, or directories using Rofi's search box. Simply type in a keyword or phrase and Rofi will return a list of results.
- Theming: Rofi is highly configurable and allows for a wide range of customization options. You can change the colors, fonts, icons, and more to fit your personal preferences.
- Keyboard navigation: Rofi has excellent keyboard support, allowing you to easily navigate through the list of results and select the one you want without ever having to touch a mouse.
- Plugin support: Rofi can be extended with plugins, allowing you to add new functionality such as calculator support or a clipboard manager.

To use Rofi, you can simply open a terminal and type "rofi" followed by any options or arguments you wish to pass. Here are some common examples:

- "rofi -show run": This will launch Rofi in run mode, allowing you to search for and launch applications from your system.
- "rofi -show drun": This will launch Rofi in application mode, allowing you to search for and launch installed applications on your system.
- "rofi -show window": This will launch Rofi in window mode, allowing you to switch between open windows on your system.
- "rofi -show combi": This will launch Rofi in combination mode, allowing you to search for and launch both applications and files/directories.
- "rofi -theme solarized": This will launch Rofi using the solarized theme, which is a popular color scheme for terminal applications. 

## tldr 
 
> An application launcher and window switcher.
> More information: <https://github.com/davatorium/rofi>.

- Show the list of apps:

`rofi -show drun`

- Show the list of all commands:

`rofi -show run`

- Switch between windows:

`rofi -show window`

- Pipe a list of items to `stdin` and print the selected item to `stdout`:

`printf "{{Choice1\nChoice2\nChoice3}}" | rofi -dmenu`
