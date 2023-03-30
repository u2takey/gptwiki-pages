# masscan 
## chatgpt 
Masscan is a open source, high-speed, TCP port scanner tool that can quickly scan large IP ranges/addresses for open ports on a network. The tool can scan IPv4 and IPv6 IP addresses and is designed to be very efficient, allowing it to scan large IP ranges in a very short time period.

The masscan command is used to run the port scanner tool. It has many options and arguments that can be used to configure the scan as per the requirement. The basic syntax of the masscan command is:

```masscan [options] <IP address or range>```

Where options can be any of the pre-defined scan options such as '-p' to specify the list of ports to be scanned, '-o' to write the output to a file, or '-iL' to read the list of IP addresses from a file.

Once the scan is initiated, the tool will begin scanning the IP addresses in the specified range for open ports. It will report back with the open ports and services running on those ports.

It is important to note that scanning a network without proper authorization is illegal, and can lead to serious consequences. Therefore, Masscan or any other port scanning tool should only be used for legitimate security testing purposes. It is highly recommended to get proper consent from the system/network owner before performing any type of scan. 

## tldr 
 
> Network scanner for scanning as fast as possible.
> Best run with elevated privileges. Nmap compatibility run `masscan --nmap` to find out more.
> More information: <https://github.com/robertdavidgraham/masscan>.

- Scan an IP or network subnet for port 80:

`masscan {{ip_address|network_prefix}} --ports {{80}}`

- Scan a class B subnet for the top 100 ports at 100,000 packets per second:

`masscan {{10.0.0.0/16}} --top-ports {{100}} --rate {{100000}}`

- Scan a class B subnet avoiding ranges from a specific exclude file:

`masscan {{10.0.0.0/16}} --top-ports {{100}} --excludefile {{path/to/file}}`

- Scan the Internet for port 443:

`masscan {{0.0.0.0/0}} --ports {{443}} --rate {{10000000}}`

- Scan the Internet for a specific port range and export to a file:

`masscan {{0.0.0.0/0}} --ports {{0-65535}} -output-format {{binary|grepable|json|list|xml}} --output-filename {{path/to/file}}`
