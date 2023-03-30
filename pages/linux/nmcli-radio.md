# nmcli radio 
## chatgpt 
The "nmcli radio" command in Linux is used to display the current state of network interfaces. It shows whether the wireless network is disabled or enabled. The output provides details about each radio interface that is available in the system. 

The "nmcli" command is used to control the NetworkManager on Linux systems. NetworkManager is a daemon that handles networking on most Linux distributions. It makes it possible to configure and manage network settings using a graphical interface, command-line tools, or scripts.

The "radio" option in the nmcli command displays information about the radio state of the system. It shows whether the network interfaces are enabled or disabled. There are typically two states for network interfaces, ON or OFF. When the interfaces are switched on, the network interfaces interface with other devices on the network, and data can be transferred. When the network interfaces are switched off, no data transfer can occur.

In summary, the "nmcli radio" command in Linux is used to display the current radio state of network interfaces. This command will show whether the network interfaces are enabled or disabled, and will provide details about each radio interface available on the system. 

## tldr 
 
> Show radio switches status or enable and disable switches.
> This subcommand can also be called with `nmcli r`.
> More information: <https://networkmanager.dev/docs/api/latest/nmcli.html>.

- Show status of Wi-Fi in NetworkManager:

`nmcli radio wifi`

- Turn Wi-Fi on or off in NetworkManager:

`nmcli radio wifi {{on|off}}`

- Show status of WWAN in NetworkManager:

`nmcli radio wwan`

- Turn WWAN on or off in NetworkManager:

`nmcli radio wwan {{on|off}}`

- Show status of both switches in NetworkManager:

`nmcli radio all`

- Turn both switches on or off in NetworkManager:

`nmcli radio all {{on|off}}`
