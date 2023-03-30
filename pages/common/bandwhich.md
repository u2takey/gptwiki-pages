# bandwhich 
## chatgpt 
Bandwhich is a CLI (Command Line Interface) tool used to analyze network bandwidth usage by different programs, processes, or connections in real-time. It displays the bandwidth usage of individual processes, connections, and ports in different colors for easy identification. It's built with Rust programming language and requires minimal CPU usage.

When the command 'bandwhich' is executed in the terminal, it launches the Bandwhich tool, and it starts monitoring your network traffic in real-time. It captures data packets that are transmitted and received by your system and analyzes their patterns to show real-time bandwidth usage for each process and connection running on the system.

The command output consists of several columns of information such as IP address, hostname, process name, protocol, port number, and the amount of network bandwidth used by each program. The tool uses different colors to distinguish different programs for better visualization.

The tool also provides different keyboard shortcuts to interact with it. For example, pressing 'p' stops the real-time update, pressing 's' sorts processes by bandwidth usage, and 'c' sorts by connections. Additionally, bandwhich provides an option to filter the output through IP addresses, ports, or process names to analyze specific network activity.

Overall, the bandwhich command is a great tool for system administrators, network engineers, and security professionals to identify bandwidth hogs, network congestion, and security threats on the network in real-time. 

## tldr 
 
> Display the current network utilization by process, connection or remote IP/hostname.
> More information: <https://github.com/imsnif/bandwhich>.

- Show the remote addresses table only:

`bandwhich --addresses`

- Show DNS queries:

`bandwhich --show-dns`

- Show total (cumulative) usage:

`bandwhich --total-utilization`

- Show the network utilization for a specific network interface:

`bandwhich --interface {{eth0}}`

- Show DNS queries with a given DNS server:

`bandwhich --show-dns --dns-server {{dns_server_ip}}`
