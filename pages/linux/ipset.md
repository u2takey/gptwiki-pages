# ipset 
## chatgpt 
The 'ipset' command is used in Linux operating systems to manage firewall rules and create and manage sets of IP addresses. It is used to configure the Linux kernel's netfilter/iptables and is capable of storing millions of IP addresses in a single set. The 'ipset' command is typically used together with the 'iptables' command, which allows one to specify a set of IP addresses for use in an iptables rule. This can be helpful when dealing with filtering traffic from multiple sources. 

Some of the tasks that can be performed with the 'ipset' command include creating and deleting sets, adding and removing elements to/from a set, displaying the contents of a set, renaming a set, and flushing all entries in a set. The 'ipset' command supports several set types, including hash:ip, hash:net, bitmap:ip, and others. 

Overall, the 'ipset' command is a powerful tool for managing firewall rules and traffic filtering on Linux systems that can help improve network security and efficiency. 

## tldr 
 
> A tool to create IP sets for firewall rules.
> More information: <https://manned.org/ipset>.

- Create an empty IP set which will contain IP addresses:

`ipset create {{set_name}} hash:ip`

- Destroy a specific IP set:

`ipset destroy {{set_name}}`

- Add an IP address to a specific set:

`ipset add {{set_name}} {{192.168.1.25}}`

- Delete a specific IP address from a set:

`ipset del {{set_name}} {{192.168.1.25}}`

- Save an IP set:

`ipset save {{set_name}} > {{path/to/ip_set}}`
