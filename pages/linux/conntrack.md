# conntrack 
## chatgpt 
The "conntrack" command is used to manipulate the network connection tracking system in the Linux kernel. This system is responsible for monitoring network connections and keeping track of information about them, such as the source and destination IP addresses, ports, and protocol used. 

The conntrack command displays information about the current connections being tracked by the system, including the number of connections, the state of each connection, and the timeout values for each connection. It can also be used to modify the timeout values and add or delete connection tracking entries. 

The conntrack command has several options, which are used to specify the type of information to display or modify, as well as the format of the output. Some of the common options include -E (display extended information), -L (list all connections), -D (delete a specific connection), and -F (flush all connections). 

Overall, conntrack is a powerful tool for managing network connections in a Linux environment, and can be useful for troubleshooting connectivity issues and monitoring network activity. 

## tldr 
 
> Interact with the Netfilter connection tracking system.
> Search, list, inspect, modify, and delete connection flows.
> More information: <https://manned.org/conntrack>.

- List all currently tracked connections:

`conntrack --dump`

- Display a real-time event log of connection changes:

`conntrack --event`

- Display a real-time event log of connection changes and associated timestamps:

`conntrack --event -o timestamp`

- Display a real-time event log of connection changes for a specific IP address:

`conntrack --event --orig-src {{ip_address}}`

- Delete all flows for a specific source IP address:

`conntrack --delete --orig-src {{ip_address}}`
