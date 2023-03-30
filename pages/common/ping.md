# ping 
## chatgpt 
"Ping" is a command that helps to check whether the network is available between one device to another device on a network. It sends a test signal to the other device, known as an ICMP (Internet Control Message Protocol) echo request packet. When the other device receives the request, it sends back an echo reply packet which confirms that it is possible to communicate. 

The "ping" command is available on many operating systems, including Windows, Mac OS, and Linux. To use it, open the command prompt or terminal and type "ping" followed by the IP address or hostname of the device you want to communicate with.

The ping command shows the round-trip time of the network packetsping, which includes sending the ICMP request, the time it takes for the other device to receive and respond, and the time it takes for the response to return to the sending machine. The time is measured in milliseconds, and the shorter it is, the better the network connection. 

In summary, the "ping" command is a useful tool for troubleshooting network connectivity issues and verifying that devices are communicating with each other on a network. 

## tldr 
 
> Send ICMP ECHO_REQUEST packets to network hosts.
> More information: <https://manned.org/ping>.

- Ping host:

`ping {{host}}`

- Ping a host only a specific number of times:

`ping -c {{count}} {{host}}`

- Ping host, specifying the interval in seconds between requests (default is 1 second):

`ping -i {{seconds}} {{host}}`

- Ping host without trying to lookup symbolic names for addresses:

`ping -n {{host}}`

- Ping host and ring the bell when a packet is received (if your terminal supports it):

`ping -a {{host}}`

- Also display a message if no response was received:

`ping -O {{host}}`
