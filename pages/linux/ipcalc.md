# ipcalc 
## chatgpt 
The `ipcalc` command is a Linux utility used for calculating various network addressing parameters of an IP address. It is used to calculate subnet masks, broadcast addresses, network addresses, and more. 

When you enter the `ipcalc` command, you must specify an IP address and its subnet mask or prefix length as an argument. The command will then generate a report that displays all the details of the IP address and subnet.

Here are some of the parameters that the `ipcalc` command can calculate:

- Network address: This is the IP address of the network itself. It is calculated by applying the subnet mask to the IP address.

- Broadcast address: This is the IP address used to broadcast messages to all devices on the network. It is calculated by inverting the subnet mask and "OR"ing it with the network address.

- Subnet mask: This is a 32-bit number used to divide the IP address into network and host bits. The `ipcalc` command will display the subnet mask in both dotted decimal and CIDR notation.

- Number of hosts: This is the total number of devices that can be connected to the network. It is calculated by subtracting the network address and broadcast address from the total number of IP addresses available in the subnet.

- Host range: This is a range of IP addresses that can be assigned to devices on the network. It is calculated by subtracting the network address and broadcast address from the total number of IP addresses available in the subnet, and then adding or subtracting 1 from each of those values.

Overall, the `ipcalc` command is a useful tool for network administrators and anyone else who needs to manage or troubleshoot network addresses. 

## tldr 
 
> Perform simple operations and calculations on IP addresses and networks.
> More information: <https://manned.org/ipcalc>.

- Show information about an address or network with a given subnet mask:

`ipcalc {{1.2.3.4}} {{255.255.255.0}}`

- Show information about an address or network in CIDR notation:

`ipcalc {{1.2.3.4}}/{{24}}`

- Show the broadcast address of an address or network:

`ipcalc -b {{1.2.3.4}}/{{30}}`

- Show the network address of provided IP address and netmask:

`ipcalc -n {{1.2.3.4}}/{{24}}`

- Display geographic information about a given IP address:

`ipcalc -g {{1.2.3.4}}`
