# wg 
## chatgpt 
The `wg` command is a tool used for managing WireGuard virtual private network (VPN) interfaces. It provides a command-line interface for configuring various aspects of the network, including setting up and managing keys, controlling access, and working with configuration files.

The `wg` command can be used to perform various operations, such as creating and configuring new interfaces, adding peers, setting up routing rules, and checking the status of the network. The basic syntax of the `wg` command is:

```
wg [command] [interface] [arguments]
```

Here, `command` refers to the action you want to perform, `interface` specifies the network interface you want to work with, and `arguments` provides any additional information or options necessary for the command to function correctly.

The most common `wg` commands include:

- `wg show`: Displays the current configuration of the specified interface, including the public and private keys, listening port, and added peers.
- `wg add`: Adds a new peer to the specified interface, including the peer's public key, allowed IP addresses, and endpoint information.
- `wg set`: Modifies the configuration of the specified interface, allowing changes to the port number, preshared keys, and other settings.
- `wg-quick`: A utility script that makes it easy to set up a basic WireGuard VPN quickly.

Overall, the `wg` command provides a powerful way to configure and manage WireGuard VPN connections using a simple and flexible command-line interface. 

## tldr 
 
> Manage the configuration of WireGuard interfaces.
> More information: <https://www.wireguard.com/quickstart/>.

- Check status of currently active interfaces:

`wg`

- Generate a new private key:

`wg genkey`

- Generate a public key from a private key:

`wg pubkey < {{path/to/private_key}} > {{path/to/public_key}}`

- Generate a public and private key:

`wg genkey | tee {{path/to/private_key}} | wg pubkey > {{path/to/public_key}}`

- Show the current configuration of a wireguard interface:

`wg showconf {{wg0}}`
