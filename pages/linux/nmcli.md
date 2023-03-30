# nmcli 
## chatgpt 
The 'nmcli' command stands for Network Manager Command-Line Interface. It is a command-line tool used to manage and control the NetworkManager daemon, which is responsible for managing network connections on Linux operating systems.

Here are a few commonly used 'nmcli' commands:

1. 'nmcli general status': This command displays the current status of the NetworkManager daemon, including whether it is running or stopped.

2. 'nmcli device show': This command provides detailed information about the network devices detected by NetworkManager, including their names, IP addresses, and hardware addresses.

3. 'nmcli connection show': This command displays a list of available network connections, including their names, types, and connection settings.

4. 'nmcli connection add': This command is used to create a new network connection profile. When creating a new connection profile, you can specify the connection type (Ethernet, Wi-Fi, VPN, etc.), connection settings, and security options.

5. 'nmcli connection modify': This command is used to modify an existing network connection profile. You can use it to change the connection settings or security options of an existing connection profile.

Overall, the 'nmcli' command is a powerful tool for managing network connections on Linux systems, and is commonly used by system administrators and advanced users alike to troubleshoot network issues and configure network settings. 

## tldr 
 
> A command-line tool for controlling NetworkManager.
> Some subcommands such as `nmcli monitor` have their own usage documentation.
> More information: <https://networkmanager.dev/docs/api/latest/nmcli.html>.

- Run an `nmcli` subcommand:

`nmcli {{agent|connection|device|general|help|monitor|networking|radio}} {{command_options}}`

- Display the current version of NetworkManager:

`nmcli --version`

- Display help:

`nmcli --help`

- Display help for a subcommand:

`nmcli {{subcommand}} --help`
