# tcpdump 
## chatgpt 
Tcpdump is a Linux command that can be used to capture network traffic. It is a packet analyzer that can filter and display network packets that are being transmitted over a network interface. 

The general syntax for using tcpdump command is:

`tcpdump [options] [filter_expression]`

Options: The options specify how the tcpdump command should operate. Some of the commonly used options include:

- `-i`: specify the network interface to capture packets from
- `-n`: display network addresses numerically instead of resolving hostnames
- `-c`: capture a specific number of packets before exiting the command
- `-s`: set the size of the packet capture buffer
- `-v`: increase the verbosity of the output

Filter_expression: The filter_expression specifies the type of packets to capture. It can be a combination of various packet fields and operators, such as:

- Host: specify a specific IP address to capture packets to/from
- Port: specify a specific port number to capture packets sent to/from
- Protocol: specify a specific protocol, such as TCP or UDP
- Direction: specify the direction of traffic, such as inbound or outbound

Examples:

- `tcpdump -i eth0`: capture packets on interface eth0
- `tcpdump -n host 192.168.1.1`: capture packets to/from IP address 192.168.1.1
- `tcpdump -i eth0 tcp port 80`: capture TCP packets on port 80 on interface eth0
- `tcpdump -i eth0 udp port 53`: capture UDP packets on port 53 on interface eth0

Tcpdump is a powerful command-line tool that can be used for troubleshooting network connectivity issues, analyzing network traffic, and debugging network applications. However, using the wrong filter_expression or capturing too much traffic can cause performance issues, so it is important to use it with caution. 

## tldr 
 
> Dump traffic on a network.
> More information: <https://www.tcpdump.org>.

- List available network interfaces:

`tcpdump -D`

- Capture the traffic of a specific interface:

`tcpdump -i {{eth0}}`

- Capture all TCP traffic showing contents (ASCII) in console:

`tcpdump -A tcp`

- Capture the traffic from or to a host:

`tcpdump host {{www.example.com}}`

- Capture the traffic from a specific interface, source, destination and destination port:

`tcpdump -i {{eth0}} src {{192.168.1.1}} and dst {{192.168.1.2}} and dst port {{80}}`

- Capture the traffic of a network:

`tcpdump net {{192.168.1.0/24}}`

- Capture all traffic except traffic over port 22 and save to a dump file:

`tcpdump -w {{dumpfile.pcap}} port not {{22}}`

- Read from a given dump file:

`tcpdump -r {{dumpfile.pcap}}`
