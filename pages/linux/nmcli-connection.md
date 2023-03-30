# nmcli connection 
## chatgpt 
The "nmcli connection" command is a Linux command that is used to manage network connections via the command-line interface. With this command, a user can view and manage all network connections running on their computer.

The "nmcli connection" command can be used to perform various tasks such as creating a new network connection, editing an existing connection, deleting a connection, activating or deactivating a particular connection, and listing available network connections.

Here are some common examples of how this command may be used:

1. nmcli connection show – This command is used to display a list of all available network connections.

2. nmcli connection add – This command is used to add a new network connection. Users can specify the connection type, settings, and other details when creating a new connection.

3. nmcli connection modify – This command is used to modify an existing network connection. Users can change the connection settings, name, or other details as needed.

4. nmcli connection delete – This command is used to delete a particular network connection.

5. nmcli connection up – This command is used to activate a specific network connection.

6. nmcli connection down – This command is used to deactivate a particular network connection.

Overall, the "nmcli connection" command is a powerful tool for managing network connections on a Linux computer from the command line. 

## tldr 
 
> Connection management with NetworkManager.
> This subcommand can also be called with `nmcli c`.
> More information: <https://networkmanager.dev/docs/api/latest/nmcli.html>.

- List all NetworkManager connections (shows name, UUID, type and device):

`nmcli connection`

- Activate a connection by specifying a UUID:

`nmcli connection up uuid {{uuid}}`

- Deactivate a connection:

`nmcli connection down uuid {{uuid}}`

- Create an auto-configured dual stack connection:

`nmcli connection add ifname {{interface_name}} type {{ethernet}} ipv4.method {{auto}} ipv6.method {{auto}}`

- Create a static IPv6-only connection:

`nmcli connection add ifname {{interface_name}} type {{ethernet}} ip6 {{2001:db8::2/64}} gw6 {{2001:db8::1}} ipv6.dns {{2001:db8::1}} ipv4.method {{ignore}}`

- Create a static IPv4-only connection:

`nmcli connection add ifname {{interface_name}} type {{ethernet}} ip4 {{10.0.0.7/8}} gw4 {{10.0.0.1}} ipv4.dns {{10.0.0.1}} ipv6.method {{ignore}}`

- Create a VPN connection using OpenVPN from a OVPN file:

`nmcli connection import type {{openvpn}} file {{path/to/vpn_config.ovpn}}`
