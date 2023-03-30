# ip neighbour 
## chatgpt 
The "ip neighbour" command is used in Linux operating systems for viewing, adding, deleting or modifying ARP (Address Resolution Protocol) table entries known as "neighbours". These entries contain the mapping of IP addresses to MAC (Media Access Control) addresses of the devices connected to the same network, allowing the devices to communicate with each other. 

The command can be used with various options such as:

1. "show" - This option displays the list of all the entries in the ARP table along with their physical address, device interface and other relevant information.
 
Example: "ip neighbour show"

2. "add" - This option is used to manually add a new entry in the ARP table. The user needs to specify the IP address and the MAC address of the new entry.

Example: "ip neighbour add 192.168.1.100 lladdr 00:11:22:33:44:55 dev eth0"

3. "del" - This option is used to delete an entry from the ARP table by specifying the IP address.

Example: "ip neighbour del 192.168.1.100"

4. "flush" - This option clears the entire ARP table.

Example: "ip neighbour flush"

Overall, the "ip neighbour" command is a useful tool for managing the ARP table and troubleshooting network connectivity issues. 

## tldr 
 
> Neighbour/ARP tables management IP subcommand.
> More information: <https://manned.org/ip-neighbour.8>.

- Display the neighbour/ARP table entries:

`ip neighbour`

- Remove entries in the neighbour table on device `eth0`:

`sudo ip neighbour flush dev {{eth0}}`

- Perform a neighbour lookup and return a neighbour entry:

`ip neighbour get {{lookup_ip}} dev {{eth0}}`

- Add or delete an ARP entry for the neighbour IP address to `eth0`:

`sudo ip neighbour {{add|del}} {{ip_address}} lladdr {{mac_address}} dev {{eth0}} nud reachable`

- Change or replace an ARP entry for the neighbour IP address to `eth0`:

`sudo ip neighbour {{change|replace}} {{ip_address}} lladdr {{new_mac_address}} dev {{eth0}}`
