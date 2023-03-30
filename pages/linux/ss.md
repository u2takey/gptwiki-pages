# ss 
## chatgpt 
The ss command is a networking utility tool used to investigate sockets, which enable network communication between a client and a server or between two servers. The name "ss" comes from the phrase "socket statistics."

The ss command provides detailed information on active network connections, including open sockets, established TCP connections, and UDP sockets. It also provides detailed information about the system's network interface, network protocols, and network interfaces that a service is using.

Here are some of the most commonly used options of the ss command:

-l: List listening sockets.
-a: Display all sockets including those that are not connected.
-o: Show the process that is associated with each socket.
-e: Show detailed information about the network connections.
-t: List only TCP sockets.
-u: List only UDP sockets.
-n: Display the numerical form of IP addresses and port numbers.

For example, to display all TCP sockets that are currently open, run the following command:

$ ss -t

This will display all established connections and listening sockets for TCP. If you want to display all sockets including those that are not connected, add the "-a" option:

$ ss -ta

Additionally, you can run ss with the "-o" option to show which process is associated with each socket. You can see the process ID (PID) and the process name, as well as the user that initiated the connection. 

Overall, the ss command is a useful tool for analyzing and debugging network connections and is typically used by system administrators and network professionals. 

## tldr 
 
> Utility to investigate sockets.
> More information: <https://manned.org/ss.8>.

- Show all TCP/UDP/RAW/UNIX sockets:

`ss -a {{-t|-u|-w|-x}}`

- Filter TCP sockets by states, only/exclude:

`ss {{state/exclude}} {{bucket/big/connected/synchronized/...}}`

- Show all TCP sockets connected to the local HTTPS port (443):

`ss -t src :{{443}}`

- Show all TCP sockets listening on the local 8080 port:

`ss -lt src :{{8080}}`

- Show all TCP sockets along with processes connected to a remote ssh port:

`ss -pt dst :{{ssh}}`

- Show all UDP sockets connected on specific source and destination ports:

`ss -u 'sport == :{{source_port}} and dport == :{{destination_port}}'`

- Show all TCP IPv4 sockets locally connected on the subnet 192.168.0.0/16:

`ss -4t src {{192.168/16}}`

- Kill IPv4 or IPv6 Socket Connection with destination IP 192.168.1.17 and destination port 8080:

`ss --kill dst {{192.168.1.17}} dport = {{8080}}`
