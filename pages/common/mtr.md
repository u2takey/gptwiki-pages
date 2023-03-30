# mtr 
## chatgpt 
mtr is a command-line tool that is used for network diagnostic and troubleshooting. It is an acronym for My Trace Route. The tool combines the functionality of two other networking tools, ping and traceroute, allowing for a comprehensive analysis of network performance and connectivity issues.

When the mtr command is executed, it sends packets of data to the specified destination address and records the time taken for the packets to reach the destination and return to the sender. It displays this information along with the hop count and round-trip time for each router or gateway along the network path.

The mtr command has several options that can be used to configure its behavior. For example, the -n option disables hostname resolution, while the -4 or -6 options can be used to specify which IP version to use for the command.

In summary, mtr is a powerful network diagnostic tool that can be used to troubleshoot connectivity issues and performance problems. Its ability to combine the functionality of ping and traceroute makes it an essential tool for network administrators and individuals who rely on stable and reliable internet connections. 

## tldr 
 
> Matt's Traceroute: combined traceroute and ping tool.
> More information: <https://bitwizard.nl/mtr>.

- Traceroute to a host and continuously ping all intermediary hops:

`mtr {{host}}`

- Disable IP address and host name mapping:

`mtr -n {{host}}`

- Generate output after pinging each hop 10 times:

`mtr -w {{host}}`

- Force IP IPv4 or IPV6:

`mtr -4 {{host}}`

- Wait for a given time (in seconds) before sending another packet to the same hop:

`mtr -i {{seconds}} {{host}}`

- Display the Autonomous System Number (ASN) for each hop:

`mtr --aslookup {{hostname}}`
