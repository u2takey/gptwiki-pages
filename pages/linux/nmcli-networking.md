# nmcli networking 
## chatgpt 
The "nmcli networking" command is used to control the NetworkManager networking service on Linux systems. The "networking" option of the "nmcli" command tool allows you to manage the state of network connectivity on your system.

The "nmcli networking" command can be used to perform various tasks related to network connectivity such as enabling or disabling networking, checking the status of network devices, and managing network connections. 

Here are some examples of how to use the "nmcli networking" command:

- To enable the networking service, run: nmcli networking on
- To disable the networking service, run: nmcli networking off
- To check the status of network devices, run: nmcli networking connectivity
- To view the list of available network interfaces, run: nmcli networking interface
- To refresh the DHCP client state on all active interfaces, run: nmcli networking dhcp
- To activate a network connection, run: nmcli networking connectivity
- To deactivate a network connection, run: nmcli networking connectivity

In summary, the "nmcli networking" command is a powerful tool for managing network connectivity on Linux systems. It allows users to enable or disable networking services, check the status of network devices, manage network connections, and more. 

## tldr 
 
> Manage the networking status of NetworkManager.
> This subcommand can also be called with `nmcli n`.
> More information: <https://networkmanager.dev/docs/api/latest/nmcli.html>.

- Show the networking status of NetworkManager:

`nmcli networking`

- Enable or disable networking and all interfaces managed by NetworkManager:

`nmcli networking {{on|off}}`

- Show the last known connectivity state:

`nmcli networking connectivity`

- Show the current connectivity state:

`nmcli networking connectivity check`
