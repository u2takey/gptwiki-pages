# nmcli general 
## chatgpt 
The "nmcli general" is a command-line tool in Linux that helps users to control and manage the network connections using the NetworkManager. Below is a detailed explanation of this command:

- "nmcli" is the NetworkManager Command-Line Interface utility in Linux that lets you control and manage the network connections from the terminal.
- "general" is a subcommand of the nmcli command, which provides the general status and information about the NetworkManager settings.

The "nmcli general" command displays various pieces of information related to NetworkManager, including:

- The version of NetworkManager installed on the system.
- The state of the NetworkManager service, whether it's running, stopped, or unknown.
- The NetworkManager's DNS configuration, showing whether it's using the system's DNS settings or custom settings.
- The NetworkManager's connectivity status, whether it's connected or disconnected.
- The overall network connectivity state, showing whether the system has fully connected, partially connected, or disconnected.

In summary, the "nmcli general" command is useful for getting an overview of the NetworkManager configuration and its connectivity status. It can be used to diagnose network problems or to verify the status of network connections. 

## tldr 
 
> Manage general settings of NetworkManager.
> This subcommand can also be called with `nmcli g`.
> More information: <https://networkmanager.dev/docs/api/latest/nmcli.html>.

- Show the general status of NetworkManager:

`nmcli general`

- Show the hostname of the current device:

`nmcli general hostname`

- Change the hostname of the current device:

`sudo nmcli general hostname {{new_hostname}}`

- Show the permissions of NetworkManager:

`nmcli general permissions`

- Show the current logging level and domains:

`nmcli general logging`

- Set the logging level and/or domains (see `man NetworkManager.conf` for all available domains):

`nmcli general logging level {{INFO|OFF|ERR|WARN|DEBUG|TRACE}} domain {{domain_1,domain_2,...}}`
