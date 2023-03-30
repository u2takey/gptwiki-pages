# nbtscan 
## chatgpt 
Nbtscan is a command-line tool used to scan and gather NetBIOS information from a network. It is a network utility used to discover hosts and services on a local network (LAN) or a wide-area network (WAN). Nbtscan works by sending NetBIOS Name Service (NBNS) protocol queries to all hosts on a network, and then collecting the responses returned by these hosts.

The syntax of the nbtscan command is as follows:
nbtscan [options] target

The "target" parameter is the IP address or the hostname of the network that you want to scan. The "options" parameter allows you to modify how the nbtscan command should be executed. Here are some of the common options used with nbtscan:

- "-h" - Displays the help menu for the nbtscan command.
- "-v" - Displays the version number of the nbtscan command.
- "-t" - Increases the timeout for each query (default=200ms).
- "-s" - Forces nbtscan to use session packets for queries.
- "-S" - Forces nbtscan to skip the NetBIOS name resolution.
- "-p" - Sets the range of ports to scan (default=1-65535).
- "-m" - Limits the number of hosts to scan at a time (default=255).

Once you have provided the target and any applicable options, the nbtscan command will execute and display the results of the scan. The output will include the NetBIOS name, IP address, and MAC address of each host that responds to the query. It may also include information about the workgroup/domain name, operating system, and open ports found on each host. 

## tldr 
 
> Scan networks for NetBIOS name information.
> More information: <https://github.com/resurrecting-open-source-projects/nbtscan>.

- Scan a network for NetBIOS names:

`nbtscan {{192.168.0.1/24}}`

- Scan a single IP address:

`nbtscan {{192.168.0.1}}`

- Display verbose output:

`nbtscan -v {{192.168.0.1/24}}`

- Display output in `/etc/hosts` format:

`nbtscan -e {{192.168.0.1/24}}`

- Read IP addresses / networks to scan from a file:

`nbtscan -f {{path/to/file.txt}}`
