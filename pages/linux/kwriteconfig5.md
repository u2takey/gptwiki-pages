# kwriteconfig5 
## chatgpt 
`kwriteconfig5` is a command line utility in the KDE Plasma desktop environment that allows users to modify or read settings in configuration files.

When you execute the `kwriteconfig5` command, it opens a configuration file editor window with the specified configuration file. You can then make changes to the configuration file and save it.

You can use `kwriteconfig5` to modify system-wide configuration files or user-specific configuration files. To modify a system-wide configuration file, you need root privileges.

Here are some examples of how to use `kwriteconfig5`:

- `kwriteconfig5 --file myapprc --group General --key SomeKey --type string "some value"`: This command sets the value of the `SomeKey` key in the `[General]` group of the `myapprc` configuration file to `"some value"`.

- `kwriteconfig5 --file kwinrc --group compositing --key OpenGLIsUnsafe --type bool true`: This command sets the boolean value of the `OpenGLIsUnsafe` key in the `[compositing]` group of the `kwinrc` configuration file to `true`.

- `kwriteconfig5 --file konsolerc --group "Desktop Entry" --key "X-DBUS-ServiceName" --type string "org.kde.konsole"`: This command sets the value of the `X-DBUS-ServiceName` key in the `[Desktop Entry]` group of the `konsolerc` configuration file to `"org.kde.konsole"`.

Overall, `kwriteconfig5` is a powerful tool for modifying configuration files in the KDE Plasma desktop environment. It allows you to customize the behavior and appearance of various applications and system components. 

## tldr 
 
> Write KConfig entries for KDE Plasma.
> More information: <https://userbase.kde.org/KDE_System_Administration/Configuration_Files>.

- Display help:

`kwriteconfig5 --help`

- Set a global configuration key:

`kwriteconfig5 --group {{group_name}} --key {{key}} {{value}}`

- Set a key in a specific configuration file:

`kwriteconfig5 --file {{path/to/file}} --group {{group_name}} --key {{key}} {{value}}`

- Delete a key:

`kwriteconfig5 --group {{group_name}} --key {{key}} --delete`

- Use systemd to start the Plasma session when available:

`kwriteconfig5 --file {{startkderc}} --group {{General}} --key {{systemdBoot}} {{true}}`

- Hide the title bar when a window is maximized (like Ubuntu):

`kwriteconfig5 --file {{~/.config/kwinrc}} --group {{Windows}} --key {{BorderlessMaximizedWindows}} {{true}}`

- Configure KRunner to open with the Meta (Command/Windows) global hotkey:

`kwriteconfig5 --file {{~/.config/kwinrc}} --group {{ModifierOnlyShortcuts}} --key {{Meta}} {{"org.kde.kglobalaccel,/component/krunner_desktop,org.kde.kglobalaccel.Component,invokeShortcut,_launch"}}`
