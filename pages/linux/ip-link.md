# ip link 
## chatgpt 
The 'ip link' command is a Linux networking command that allows you to manage network interfaces. It provides information about the network interfaces available on your system, allows you to configure, enable, or disable them, set network parameters like IP address, netmask, and routing tables. Some common options for the 'ip link' command are:

- 'show': The 'show' subcommand displays the network interfaces on your system along with various details like their name, state, MAC address, and MTU (maximum transmission unit).
- 'set': The 'set' subcommand allows you to modify the configuration of a network interface. For example, you can change the MTU or enable/disable the interface.
- 'up'/'down': The 'up' and 'down' subcommands allow you to enable or disable a network interface respectively.
- 'add': The 'add' subcommand is used to add a new network interface to your system, like a virtual interface.
- 'delete': The 'delete' subcommand is used to remove a network interface from your system.

Overall, the 'ip link' command is a powerful tool for managing network interfaces on a Linux system. It is useful for debugging connectivity issues, setting up networking interfaces for virtual machines, and configuring network settings for various applications. 

## tldr 
 
> Manage network interfaces.
> More information: <https://man7.org/linux/man-pages/man8/ip-link.8.html>.

- Show information about all network interfaces:

`ip link`

- Show information about a specific network interface:

`ip link show {{ethN}}`

- Bring a network interface up or down:

`ip link set {{ethN}} {{up|down}}`

- Give a meaningful name to a network interface:

`ip link set {{ethN}} alias "{{LAN Interface}}"`

- Change the MAC address of a network interface:

`ip link set {{ethN}} address {{ff:ff:ff:ff:ff:ff}}`

- Change the MTU size for a network interface to use jumbo frames:

`ip link set {{ethN}} mtu {{9000}}`
