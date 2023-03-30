# brctl 
## chatgpt 
The brctl command is a Linux command that is used for configuring and managing Ethernet bridge interfaces. This command is typically used to create and manage virtual network interfaces and is especially useful when creating complex network topologies. Here is a breakdown of some of the common options and functions of the brctl command:

- create: This option is used to create a new bridge interface, for example:
    - brctl create bridge_name

- addif: This option is used to add a network interface to a bridge, for example:
    - brctl addif bridge_name eth0

- show: This option is used to display information about the bridge interfaces that exist on the system, for example:
    - brctl show

- delbr: This option is used to delete a bridge interface, for example:
    - brctl delbr bridge_name

- delif: This option is used to remove a network interface from a bridge, for example:
    - brctl delif bridge_name eth0

Overall, the brctl command is a powerful tool for managing and configuring network interfaces on Linux systems, and is especially useful for creating virtual network interfaces and managing complex network topologies. 

## tldr 
 
> Ethernet bridge administration.
> More information: <https://manned.org/brctl>.

- Show a list with information about currently existing Ethernet bridges:

`sudo brctl show`

- Create a new Ethernet bridge interface:

`sudo brctl add {{bridge_name}}`

- Delete an existing Ethernet bridge interface:

`sudo brctl del {{bridge_name}}`

- Add an interface to an existing bridge:

`sudo brctl addif {{bridge_name}} {{interface_name}}`

- Remove an interface from an existing bridge:

`sudo brctl delif {{bridge_name}} {{interface_name}}`
