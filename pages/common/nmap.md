# nmap 
## chatgpt 
Nmap stands for "Network Mapper". It is a free and open-source network exploration and security auditing tool. It is used to discover hosts and services on a computer network, thus creating a "map" of the network. Nmap can be used to gather information, scan for open ports and detect potential vulnerabilities on a network.

The basic syntax of the nmap command is:

```
nmap [Scan Type] [Options] [Target]
```

Some common options used with nmap are:

- `-sS`: a stealth scan, the default scan type of nmap.
- `-sT`: a TCP connect scan, which simulates the opening of a connection to a target host.
- `-sU`: a UDP scan, which determines which UDP ports are open on a target host.
- `-A`: enables OS detection, version detection, script scanning, and Traceroute.
- `-p`: specifies the port range to scan.
- `-O`: performs OS detection on the target host.

Example usage of Nmap:

```
nmap -sS -p 1-100 192.168.1.1
```

This command scans the first 100 ports (-p 1-100) of the IP address 192.168.1.1 using a stealth scan (-sS). It will show any open ports, and can give an idea about the services running on those ports. 

Nmap is a powerful tool that can be used both for network exploration and network security auditing. It is important to use it carefully and only on systems that you have permission to scan. 

## tldr 
 
> Network exploration tool and security / port scanner.
> Some features only activate when Nmap is run with root privileges.
> More information: <https://nmap.org>.

- Check if an IP address is up, and guess the remote host's operating system:

`nmap -O {{ip_or_hostname}}`

- Try to determine whether the specified hosts are up (ping scan) and what their names are:

`nmap -sn {{ip_or_hostname}} {{optional_another_address}}`

- Also enable scripts, service detection, OS fingerprinting and traceroute:

`nmap -A {{address_or_addresses}}`

- Scan a specific list of ports (use '-p-' for all ports from 1 to 65535):

`nmap -p {{port1,port2,...,portN}} {{address_or_addresses}}`

- Perform service and version detection of the top 1000 ports using default NSE scripts; writing results ('-oN') to output file:

`nmap -sC -sV -oN {{top-1000-ports.txt}} {{address_or_addresses}}`

- Scan target(s) carefully using 'default and safe' NSE scripts:

`nmap --script "default and safe" {{address_or_addresses}}`

- Scan web server running on standard ports 80 and 443 using all available 'http-*' NSE scripts:

`nmap --script "http-*" {{address_or_addresses}} -p 80,443`

- Perform a stealthy very slow scan ('-T0') trying to avoid detection by IDS/IPS and use decoy ('-D') source IP addresses:

`nmap -T0 -D {{decoy1_ipaddress,decoy2_ipaddress,...,decoyN_ipaddress}} {{address_or_addresses}}`
