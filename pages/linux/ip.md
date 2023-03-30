# ip 
## chatgpt 
The "ip" command is a powerful network utility tool that is available in modern Linux operating systems. It is used to manage, configure, and troubleshoot various network components such as interfaces, routes, and addresses, among other things.

Some of the common tasks that can be performed using the "ip" command include adding and deleting network interfaces or aliases, changing interface addresses, configuring network routes, setting up virtual private networks (VPNs), and managing network namespaces. The syntax of the "ip" command varies depending on the particular task being performed, and it typically involves specifying one or more options and respective arguments.

Overall, the "ip" command is a versatile and essential tool for network administrators who wish to keep their systems running smoothly and efficiently. With its many features and capabilities, it helps to simplify the management of complex network configurations and to troubleshoot issues as they arise. 

## tldr 
 
> Show / manipulate routing, devices, policy routing and tunnels.
> Some subcommands such as `ip address` have their own usage documentation.
> More information: <https://www.man7.org/linux/man-pages/man8/ip.8.html>.

- List interfaces with detailed info:

`ip address`

- List interfaces with brief network layer info:

`ip -brief address`

- List interfaces with brief link layer info:

`ip -brief link`

- Display the routing table:

`ip route`

- Show neighbors (ARP table):

`ip neighbour`

- Make an interface up/down:

`ip link set {{interface}} up/down`

- Add/Delete an IP address to an interface:

`ip addr add/del {{ip}}/{{mask}} dev {{interface}}`

- Add a default route:

`ip route add default via {{ip}} dev {{interface}}`
