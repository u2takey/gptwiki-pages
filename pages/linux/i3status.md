# i3status 
## chatgpt 
i3status is a command used to display system information and status bar in the i3 window manager. It is a small program that runs in the background and periodically collects and updates information about the system's status, such as CPU usage, memory usage, disk usage, date and time, battery status, weather, and more.

By default, the i3status command outputs the status information to the command line interface (CLI). However, it can also be configured to output to the i3 status bar, which is a simple bar located at the top or bottom of the i3 window that displays system information and other relevant data.

The i3status command can be customized to fit the user's preferences and needs. This is done by creating a configuration file in the user's home directory called '.i3status.conf', which contains options and settings for the i3status command.

Overall, the i3status command is an important tool for keeping track of important system information and keeping the user informed about the status of their system. 

## tldr 
 
> Status line for the i3 window manager.
> This command is usually called from the i3 configuration file.
> More information: <https://i3wm.org/i3status/manpage.html>.

- Print the status line to `stdout` periodically, using the default configuration:

`i3status`

- Print the status line to `stdout` periodically, using a specific configuration:

`i3status -c {{path/to/i3status.conf}}`

- Display the `i3status` version and help:

`i3status -h`
