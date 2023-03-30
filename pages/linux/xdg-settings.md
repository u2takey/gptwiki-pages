# xdg-settings 
## chatgpt 
The xdg-settings command is a command-line tool that is used to set the default values of various desktop-related settings. This command works with the XDG base directory specification, a set of standards for the organization and management of user-specific configuration, data, cache, and runtime files.

There are several options available with the xdg-settings command, including:

- get: This option is used to get the current value of a setting. For example, xdg-settings get default-web-browser will return the default web browser currently set in the system.

- set: This option is used to set a new value for a setting. For example, xdg-settings set default-web-browser firefox.desktop will set Firefox as the default web browser for the system.

- check: This option is used to check if a particular setting is supported by the desktop environment or not. For example, xdg-settings check default-web-browser will return whether the desktop environment supports setting the default web browser or not.

- list: This option is used to list all the settings that can be modified using the xdg-settings command.

The xdg-settings command is mostly used in shell scripts or automated setup processes to configure system settings. This command is also helpful in ensuring consistency across different desktop environments and Linux distributions. 

## tldr 
 
> Manage settings of XDG-compatible desktop environments.
> More information: <https://portland.freedesktop.org/doc/xdg-settings.html>.

- Print the default web browser:

`xdg-settings get {{default-web-browser}}`

- Set the default web browser to Firefox:

`xdg-settings set {{default-web-browser}} {{firefox.desktop}}`

- Set the default mail URL scheme handler to Evolution:

`xdg-settings set {{default-url-scheme-handler}} {{mailto}} {{evolution.desktop}}`

- Set the default PDF document viewer:

`xdg-settings set {{pdf-viewer.desktop}}`

- Display help:

`xdg-settings --help`
