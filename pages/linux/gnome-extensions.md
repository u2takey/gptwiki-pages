# gnome-extensions 
## chatgpt 
gnome-extensions is a command used in Linux systems to manage extensions on the GNOME desktop environment. GNOME is a user-friendly and customizable desktop environment with various features that help to improve productivity.

This command allows the user to download, install, enable, disable, and remove extensions from the GNOME shell. GNOME extensions let users add new functionality to their desktops, such as weather forecasts, system monitoring tools, or video player controls.

The gnome-extensions command can be used in the terminal, and the available options include:

- List: This option displays a list of installed extensions.
- Info: This option shows detailed information about a specific extension.
- Enable: This option enables a specific extension.
- Disable: This option disables a specific extension.
- Create: This option creates a new extension.
- Remove: This option removes an extension from the system.

Overall, gnome-extensions command provides a convenient way to manage, configure and personalize the GNOME desktop environment according to users' preferences. 

## tldr 
 
> Manage gnome extensions from the terminal.
> More information: <https://wiki.gnome.org/Projects/GnomeShell/Extensions>.

- Display the version:

`gnome-extensions version`

- List all the installed extensions:

`gnome-extensions list`

- Display information about a specific extension:

`gnome-extensions info "{{extension_id}}"`

- Display help for a subcommand (like `list`):

`gnome-extensions help {{subcommand}}`

- Enable a specific extension:

`gnome-extensions enable "{{extension_id}}"`

- Disable a specific extension:

`gnome-extension disable "{{extension_id}}"`

- Uninstall a specific extension:

`gnome-extension uninstall "{{extension_id}}"`
