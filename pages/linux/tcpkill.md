# tcpkill 
## chatgpt 
The 'tcpkill' command is a Linux networking utility that allows users to kill a TCP connection between two machines. 

The syntax of the command is:

tcpkill [-i interface] [-9] [expression]

Where:
- [-i interface]: specifies the interface to listen on.
- [-9]: forces the connection to close immediately.
- [expression]: a BPF filter expression to match packets to kill.

The tcpkill command is used for troubleshooting network connectivity issues or for closing rogue TCP connections. 

For example, to kill all TCP connections between two machines with IP addresses 192.168.1.2 and 192.168.1.3 on the enp0s3 interface, the command would be:

tcpkill -i enp0s3 host 192.168.1.2 and 192.168.1.3

This would kill all TCP connections between the two machines, allowing them to start fresh and establish new connections. 

It should be noted that the 'tcpkill' command requires administrative privileges, and should be used with caution as it can disrupt network traffic and cause unintended consequences. 

## tldr 
 
> Kills specified in-progress TCP connections.
> More information: <https://manned.org/tcpkill>.

- Kill in-progress connections at a specified interface, host and port:

`tcpkill -i {{eth1}} host {{192.95.4.27}} and port {{2266}}`
