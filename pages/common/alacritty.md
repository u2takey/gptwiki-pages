# alacritty 
## chatgpt 
"Alacritty" is a command that launches a terminal emulator application, also called Alacritty. Alacritty is a cross-platform, GPU-accelerated terminal emulator that is built using Rust programming language, and offers a modern look and feel with a high level of performance.

When you run the "alacritty" command, it will open a new window that provides a command-line interface (CLI) to your operating system. The window will resemble the default command-line interface that comes with your operating system, but with a more modern and customizable appearance. You can use the Alacritty terminal emulator to execute various commands, run scripts, and compile code, just like any other CLI.

Alacritty offers many features and options that you can customize based on your preferences. For example, you can change font size, modify color schemes, and configure keyboard shortcuts. It also offers features such as scrollback and tabbed interface, which makes it easy to navigate between different terminal sessions.

In summary, the "alacritty" command launches a fast, modern, and customizable terminal emulator, allowing you to interact with your operating system through a command-line interface. 

## tldr 
 
> Cross-platform, GPU-accelerated terminal emulator.
> More information: <https://github.com/alacritty/alacritty>.

- Open a new Alacritty window:

`alacritty`

- Run in a specific directory:

`alacritty --working-directory {{path/to/directory}}`

- Run a command in a new Alacritty window:

`alacritty -e {{command}}`

- Specify alternative configuration file (defaults to `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):

`alacritty --config-file {{path/to/config.yml}}`

- Run with live config reload enabled (can also be enabled by default in `alacritty.yml`):

`alacritty --live-config-reload --config-file {{path/to/config.yml}}`
