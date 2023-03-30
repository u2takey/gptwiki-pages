# netstat 
## chatgpt 
Netstat is a command-line utility that displays active connections and network statistics on a computer. It is a basic networking tool that is available in most operating systems like Linux, Windows, and macOS.

The netstat command can be used with various options to retrieve different types of information. Here are some of its most commonly used options:

- netstat -a: Displays all active connections and their status, including those that are listening for incoming connections.

- netstat -n: Displays the addresses and port numbers in numerical form, rather than automatically resolving host and service names.

- netstat -p: Displays the process ID (PID) associated with each connection or socket.

- netstat -r: Displays the routing table for the computer, showing how network traffic is being routed.

- netstat -s: Displays statistics for each protocol, such as the number of packets sent and received, errors, and discards.

- netstat -t: Displays the current TCP connections.

- netstat -u: Displays the current UDP connections.

By default, the netstat command displays information for all protocol types. However, you can limit the output to specific protocols, such as TCP, UDP, or ICMP, by using the appropriate options.

Overall, netstat is a useful tool for troubleshooting network issues, checking for suspicious activity, and monitoring network performance. 

## tldr 
 
> Displays network-related information such as open connections, open socket ports, etc.
> More information: <https://man7.org/linux/man-pages/man8/netstat.8.html>.

- List all ports:

`netstat --all`

- List all listening ports:

`netstat --listening`

- List listening TCP ports:

`netstat --tcp`

- Display PID and program names:

`netstat --program`

- List information continuously:

`netstat --continuous`

- List routes and do not resolve IP addresses to hostnames:

`netstat --route --numeric`

- List listening TCP and UDP ports (+ user and process if you're root):

`netstat --listening --program --numeric --tcp --udp --extend`
