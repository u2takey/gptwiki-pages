# route 
## chatgpt 
The "route" command is used to view and modify the network routing table on a computer. The routing table is a set of rules that determine how data packets travel from one network to another. 

The basic syntax of the "route" command is as follows:

route [-f] [-p] [command [destination] [mask Netmask] [gateway] [metric Metric]] 

The meanings of some important options and arguments are:

- "-f": Clears the routing table and deletes all entries.
- "-p": Adds a persistent (static) route to the routing table. By default, routes added using the "route" command are not persistent and will be lost when the computer is restarted.
- "command": Specifies the action to be taken on the routing table, such as adding, deleting or modifying a route. The most common commands are "add", "delete" and "change".
- "destination": Specifies the IP address or network address of the destination network for which the route is being added or modified.
- "mask Netmask": Specifies the subnet mask for the destination network.
- "gateway": Specifies the IP address of the next-hop router that the data packets should be forwarded to en route to the destination network.
- "metric Metric": Specifies the cost of the route or the number of hops to the destination network. Lower metric values indicate higher priorities.

In summary, the "route" command is an important tool for managing network routes and traffic flows on a computer. It can be used to diagnose connectivity issues, configure routing policies, and optimize network performance. 

## tldr 
 
> Use route cmd to set the route table.
> More information: <https://manned.org/route>.

- Display the information of route table:

`route -n`

- Add route rule:

`sudo route add -net {{ip_address}} netmask {{netmask_address}} gw {{gw_address}}`

- Delete route rule:

`sudo route del -net {{ip_address}} netmask {{netmask_address}} dev {{gw_address}}`
