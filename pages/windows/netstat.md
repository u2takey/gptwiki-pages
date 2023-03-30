# netstat 
## chatgpt 
Netstat is a command-line utility tool used in networking to display various information and statistics about network connections, active ports, active TCP/UDP connections, and network protocols. The tool is available in most major operating systems, including Windows, Linux, and macOS.

The netstat command provides different options and syntax, which serve various purposes. Some of them are:

- `netstat -a`: This command shows all active TCP and UDP connections on the system.

- `netstat -n`: This command shows active network connections in numerical form. 

- `netstat -b`: This command shows the process ID and name that are listening or using the ports.

- `netstat -e`: This command shows Ethernet statistics, such as the number of bytes sent and received over the network.

- `netstat -r`: This command displays the routing information, including the default gateway, routing tables, and interface information.

Overall, the netstat command is a useful tool for network administrators to monitor and troubleshoot various networking issues. It can help identify active connections, check for any unusual network behavior or traffic patterns, and diagnose potential network congestion or performance issues. 

## tldr 
 
> Displays active TCP connections, ports on which the computer is listening, network adapter statistics, the IP routing table, IPv4 statistics and IPv6 statistics.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/netstat>.

- Display active TCP connections:

`netstat`

- Display all active TCP connections and the TCP and UDP ports on which the computer is listening:

`netstat -a`

- Display network adapter statistics, such as the number of bytes and packets sent and received:

`netstat -e`

- Display active TCP connections and express addresses and port numbers numerically:

`netstat -n`

- Display active TCP connections and include the process ID (PID) for each connection:

`netstat -o`

- Display the contents of the IP routing table:

`netstat -r`

- Display statistics by protocol:

`netstat -s`

- Display a list of currently open ports and related IP addresses:

`netstat -an`
