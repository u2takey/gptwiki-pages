# ip address 
## chatgpt 
The command "ip address" is used in networking on Linux and Unix operating systems to view or configure the IP address of a network interface. When executed, this command displays the IP address, subnet mask, and broadcast address of all configured network interfaces on the system. It also displays the MTU (Maximum Transmission Unit) size and other relevant information.

Here is a breakdown of the syntax and usage of the "ip address" command:

Syntax:
ip address [show | add | del] [interface name] [options]

Usage:
- "ip address show" allows you to view current IP address configurations on all interfaces.
- "ip address add" allows you to add a new IP address to an interface.
- "ip address del" allows you to delete an existing IP address from an interface.

Options:
- "dev" or "interface name" - specifies the interface name for which you want to view or configure IP address details.
- "inet" - specifies that IPv4 addresses should be displayed or configured.
- "inet6" - specifies that IPv6 addresses should be displayed or configured.
- "scope" - specifies the scope of the IP address.
- "label" - specifies a label for the IP address, which can help you identify it later.
- "broadcast" - specifies the broadcast address for the network interface.
- "netmask" - specifies the subnet mask for the network interface.
- "up" or "down" - enables or disables the interface, respectively. 

## tldr 
 
> IP Address management subcommand.
> More information: <https://manned.org/ip-address>.

- List network interfaces and their associated IP addresses:

`ip address`

- Filter to show only active network interfaces:

`ip address show up`

- Display information about a specific network interface:

`ip address show dev {{eth0}}`

- Add an IP address to a network interface:

`ip address add {{ip_address}} dev {{eth0}}`

- Remove an IP address from a network interface:

`ip address delete {{ip_address}} dev {{eth0}}`

- Delete all IP addresses in a given scope from a network interface:

`ip address flush dev {{eth0}} scope {{global|host|link}}`
