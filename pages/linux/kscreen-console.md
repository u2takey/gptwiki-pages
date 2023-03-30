# kscreen-console 
## chatgpt 
`kscreen-console` is a command that is used in the KDE Plasma desktop environment to provide a command-line interface for managing display configurations. It allows you to configure your monitor settings, create or modify profiles, and view information about your display hardware.

When the `kscreen-console` command is executed in a terminal, it launches a graphical interface that provides several options for managing display configurations. Some of the common tasks that can be performed with `kscreen-console` include:

1. Listing available displays: By running `kscreen-console --list`, you can get a list of all the available displays connected to your system.

2. Setting up new profiles: You can create new display profiles or modify existing ones using `kscreen-console --profile`. You can specify different resolutions, refresh rates, and other settings.

3. Enabling or disabling displays: Using `kscreen-console --output`, you can enable or disable a specific display.

4. Adjusting orientation and position: You can change the orientation and position of a display using `kscreen-console --position` and `kscreen-console --rotate`.

5. Saving and loading profiles: The `kscreen-console --save` and `kscreen-console --load` commands are used to save or load display profiles from your system.

Overall, `kscreen-console` is a useful tool for managing display configurations in a KDE Plasma desktop environment, and it can be particularly helpful for users who prefer to work from the terminal. 

## tldr 
 
> Command-line tool to query KScreen's status.
> More information: <https://manned.org/kscreen-console>.

- Show all outputs and configuration files to attach to a bug report:

`kscreen-console bug`

- Show paths to KScreen configuration files:

`kscreen-console config`

- Show KScreen output information and configuration:

`kscreen-console outputs`

- Monitor for changes:

`kscreen-console monitor`

- Show the current KScreen configuration as JSON:

`kscreen-console json`

- Display help:

`kscreen-console --help`

- Display help including Qt specific command-line options:

`kscreen-console --help-all`
