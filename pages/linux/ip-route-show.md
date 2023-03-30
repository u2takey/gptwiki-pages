# ip route show 
## chatgpt 
The `ip route show` command is a Linux networking command that is used to display the current routing table on your system. 

The `ip` command is a powerful tool that allows the user to manage networking interfaces, network addresses, and routing tables. 

The `route` commands display the system's routing table, which is a crucial component of any network. It contains information on how packets should be directed from one network segment to another. By default, when the `show` option is used with the `ip route` command, it displays the currently configured routing table on the system.

The information displayed by this command includes the destination network or host, netmask, gateway, metric and interface. 

- Destination: the address or network of the destination host. 
- Netmask: the subnet mask or network mask for the network.
- Gateway: the IP address of the gateway router that traffic for that destination will be routed through. 
- Metric: the routing metric, which is used to determine the best path to a destination network. 
- Interface: the name of the network interface associated with the route.

Overall, the `ip route show` command plays a critical role in troubleshooting network issues, analyzing network performance, and managing network circulation. 

## tldr 
 
> Display subcommand for IP Routing table management.
> More information: <https://manned.org/ip-route>.

- Display the routing table:

`ip route show`

- Display the main routing table (same as first example):

`ip route show {{main|254}}`

- Display the local routing table:

`ip route show table {{local|255}}`

- Display all routing tables:

`ip route show table {{all|unspec|0}}`

- List routes from a given device only:

`ip route show dev {{eth0}}`

- List routes within a given scope:

`ip route show scope link`

- Display the routing cache:

`ip route show cache`

- Display only IPv6 or IPv4 routes:

`ip {{-6|-4}} route show`
