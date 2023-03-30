# lxc network 
## chatgpt 
The `lxc network` command is a sub-command of the Linux Containers (LXC) tool that provides network-related operations for LXC networking. This command enables the creation, management, and deletion of LXC networks that are used to provide network connectivity for LXC containers.

Here are some of the sub-commands and their functions:

- `lxc network create`: This sub-command enables the creation of a new LXC network. This command can be used to create a new bridge, or an existing bridge can be used to create a new network.

- `lxc network list`: This sub-command lists all the available LXC networks in the system. It displays information such as network name, driver, and subnet.

- `lxc network show`: This sub-command provides detailed information about a specific LXC network. It displays information such as network name, driver, subnet, and whether it is managed or not.

- `lxc network edit`: This sub-command allows you to edit a specific LXC network's configuration, such as adding or removing a subnet, changing the network driver, or setting the MTU.

- `lxc network delete`: This sub-command allows you to delete a specific LXC network. It removes all containers connected to the network and then deletes the network itself.

In summary, the `lxc network` command is a tool used for managing LXC network configurations, which are used to provide network connectivity to LXC containers. 

## tldr 
 
> Manage networks for LXD containers.
> More information: <https://linuxcontainers.org/lxd/docs/master/networks>.

- List all available networks:

`lxc network list`

- Show the configuration of a specific network:

`lxc network show {{network_name}}`

- Add a running instance to a specific network:

`lxc network attach {{network_name}} {{container_name}}`

- Create a new managed network:

`lxc network create {{network_name}}`

- Set a bridge interface of a specific network:

`lxc network set {{network_name}} bridge.external_interfaces {{eth0}}`

- Disable NAT for a specific network:

`lxc network set {{network_name}} ipv{{4}}.nat false`
