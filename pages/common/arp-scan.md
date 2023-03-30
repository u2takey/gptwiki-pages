# arp-scan 
## chatgpt 
The "arp-scan" command is a network utility tool that is used to send and receive Address Resolution Protocol (ARP) packets over the network. ARP protocol enables a device to map a Network Layer IP address to a Physical Layer hardware address in a Local Area Network (LAN).

Here is a detailed explanation of the command:

Syntax:
arp-scan [ options ] [ targets... ]

Arguments:
• targets: Specifies the target IP addresses or the network IP addresses to be scanned.

Options:
• -I {interface}: Specifies the network interface to be used, the default network interface is used if not specified.
• -s {ip_address}: Specifies the IP address to use as the source address in outgoing ARP packets.
• -l: Shows the local network host list.
• -v: Turns on verbose mode.
• -f {filename}: Reads the target IP addresses or the network IP addresses from a file.
• -q: Operates quietly with no output to the console.
• -S: Displays MAC addresses in colon-separated format.
• -p: Specifies whether the target host is present or not.

Example:
To perform an ARP scan on the local network, use the command:

arp-scan -l

This will scan the entire local network and display the IP addresses along with the corresponding MAC addresses of all the devices connected to the network. 

Another example, if you want to scan all the IP addresses in the 192.168.1.0/24 subnet, use the command:

arp-scan 192.168.1.0/24

This will send ARP packets to all the IP addresses in the specified subnet and displays the result with corresponding MAC addresses of the hosts that responded. 

Note: The arp-scan command requires root privileges to execute successfully. It can be installed on various operating systems like Linux, macOS, and Windows. 

## tldr 
 
> Send ARP packets to hosts (specified as IP addresses or hostnames) to scan the local network.
> More information: <https://github.com/royhills/arp-scan>.

- Scan the current local network:

`arp-scan --localnet`

- Scan an IP network with a custom bitmask:

`arp-scan {{192.168.1.1}}/{{24}}`

- Scan an IP network within a custom range:

`arp-scan {{127.0.0.0}}-{{127.0.0.31}}`

- Scan an IP network with a custom net mask:

`arp-scan {{10.0.0.0}}:{{255.255.255.0}}`
