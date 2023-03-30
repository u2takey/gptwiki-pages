# ip route 
## chatgpt 
The `ip route` command is a Linux networking command that is used to view and manipulate the routing table of the system. The routing table is used by the system to determine the path that network traffic takes to reach its destination.

The command has several options, including:

- `show`: This option is used to display the current routing table.
- `add`: This option is used to add a new route to the routing table.
- `delete`: This option is used to delete a route from the routing table.
- `change`: This option is used to modify an existing route in the routing table.

The syntax for the `ip route` command is as follows:

```
ip route [option] [target] [gateway] [netmask]
```

- `option`: Specifies the action to be taken on the routing table, such as "show", "add", "delete", or "change".
- `target`: Specifies the destination network address.
- `gateway`: Specifies the IP address of the gateway through which traffic should be sent.
- `netmask`: Specifies the network mask for the destination network.

For example, the command `ip route show` will display the current routing table, while the command `ip route add 192.168.1.0/24 via 10.0.0.1` will add a new route to the routing table that specifies that traffic destined for the network 192.168.1.0/24 should be sent via the gateway at 10.0.0.1. 

## tldr 
 
> IP Routing table management subcommand.
> More information: <https://manned.org/ip-route>.

- Display the routing table:

`ip route {{show|list}}`

- Add a default route using gateway forwarding:

`sudo ip route add default via {{gateway_ip}}`

- Add a default route using `eth0`:

`sudo ip route add default dev {{eth0}}`

- Add a static route:

`sudo ip route add {{destination_ip}} via {{gateway_ip}} dev {{eth0}}`

- Delete a static route:

`sudo ip route del {{destination_ip}} dev {{eth0}}`

- Change or replace a static route:

`sudo ip route {{change|replace}} {{destination_ip}} via {{gateway_ip}} dev {{eth0}}`

- Show which route will be used by the kernel to reach an IP address:

`ip route get {{destination_ip}}`
