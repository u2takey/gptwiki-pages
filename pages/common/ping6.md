# ping6 
## chatgpt 
ping6 is a command line utility used for testing connectivity between two network devices using the Internet Protocol version 6 (IPv6) address format. It works similarly to the ping command used for IPv4.

The ping6 command sends a series of ICMPv6 (Internet Control Message Protocol version 6) echo requests to a specified destination IPv6 address and measures the response time to determine the network latency and packet loss. The command also provides useful information about the overall network performance, including the round-trip time (RTT), packets transmitted and received, and any error messages.

To use the ping6 command, open a terminal or command prompt and type "ping6" followed by the IPv6 address of the destination device. For example, "ping6 2001:db8::1" will send ICMPv6 echo requests to the IPv6 address 2001:db8::1.

The ping6 command offers several options, such as specifying the number of ICMPv6 packets to send, adjusting the time period between each request, and setting the maximum amount of time the command waits for a response before timing out.

Overall, ping6 is a useful tool for network administrators and users who need to diagnose network connectivity issues or test the performance of their IPv6 network. 

## tldr 
 
> Send ICMP ECHO_REQUEST packets to network hosts via IPv6 address.
> More information: <https://manned.org/ping6>.

- Ping a host:

`ping6 {{host}}`

- Ping a host only a specific number of times:

`ping6 -c {{count}} {{host}}`

- Ping a host, specifying the interval in seconds between requests (default is 1 second):

`ping6 -i {{seconds}} {{host}}`

- Ping a host without trying to lookup symbolic names for addresses:

`ping6 -n {{host}}`

- Ping a host and ring the bell when a packet is received (if your terminal supports it):

`ping6 -a {{host}}`
