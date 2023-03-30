# gsettings 
## chatgpt 
The `gsettings` command is used in the Linux operating system to interact with the GSettings configuration system. GSettings is a mechanism for storing and retrieving key-value pairs of configuration data for GNOME applications.

When you run the `gsettings` command, you can specify a schema name, a key path, and an optional value. The schema name represents a group of related settings, while the key path represents a specific setting within that group.

For example, the following command retrieves the current wallpaper setting in GNOME:

```
gsettings get org.gnome.desktop.background picture-uri
```

In this command, `org.gnome.desktop.background` is the schema name, and `picture-uri` is the key path for the wallpaper setting.

You can also use the `set` subcommand to change a configuration value. For example, the following command sets the wallpaper to a specific image:

```
gsettings set org.gnome.desktop.background picture-uri 'file:///path/to/image.jpg'
```

Note that the value for the `picture-uri` key is a file URL that points to the location of the image file on the local file system.

The `gsettings` command can be used to view and modify a wide range of GNOME settings, including desktop backgrounds, keyboard shortcuts, window behavior, screen resolution, and more. It can also be used in shell scripts and other automated processes to configure system settings programmatically. 

## tldr 
 
> Query and modify dconf settings with schema validation.
> More information: <https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/8/html/using_the_desktop_environment_in_rhel_8/configuring-gnome-at-low-level_using-the-desktop-environment-in-rhel-8#using-gsettings-command_configuring-gnome-at-low-level>.

- Set the value of a key. Fails if the key doesn't exist or the value is out of range:

`gsettings set {{org.example.schema}} {{example-key}} {{value}}`

- Print the value of a key or the schema-provided default if the key has not been set in `dconf`:

`gsettings get {{org.example.schema}} {{example-key}}`

- Unset a key, so that its schema default value will be used:

`gsettings reset {{org.example.schema}} {{example-key}}`

- Display all (non-relocatable) schemas, keys, and values:

`gsettings list-recursively`

- Display all keys and values (default if not set) from one schema:

`gsettings list-recursively {{org.example.schema}}`

- Display schema-allowed values for a key (helpful with enum keys):

`gsettings range {{org.example.schema}} {{example-key}}`

- Display the human-readable description of a key:

`gsettings describe {{org.example.schema}} {{example-key}}`
