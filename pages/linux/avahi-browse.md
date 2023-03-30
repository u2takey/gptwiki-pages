# avahi-browse 
## chatgpt 
Avahi-browse is a command-line utility that is part of the Avahi package. Avahi is a zero-configuration networking (zeroconf) protocol suite that is designed to make it easy to discover services and devices on a local network. The avahi-browse utility allows you to browse network services published by other devices on the local network.

Here is a breakdown of the avahi-browse command:

Syntax: avahi-browse [options] [service type]

Options:

- -a, --all: List all available services instead of stopping after the first match.
- -t, --terminate: Terminate after the first match or after a timeout has occurred.
- -p, --parsable: Produce output in a machine-readable format.
- -f, --full: Display all available information, including the IP address of the server and the port number being used for each service.
- -r, --resolve: Resolve service names to IP addresses.
- -v, --verbose: Enable verbose output.

Service Type: This is the type of service you want to browse for. For example, if you want to browse for all available printers on the network, you would use the service type "ipp" (Internet Printing Protocol).

Example:

To browse for all available printers on the network, you would run the following command:

avahi-browse -a -t _ipp._tcp

This command will list all available printers on the network, and it will terminate the browse operation after the first match or after a timeout has occurred. The "-t" option is optional, but it can be useful if you only want to see the first available service. The "_ipp._tcp" parameter specifies the service type (Internet Printing Protocol over TCP) that we want to browse for. 

## tldr 
 
> Displays services and hosts exposed on the local network via mDNS/DNS-SD.
> Avahi is compatible with Bonjour (Zeroconf) found in Apple devices.
> More information: <https://www.avahi.org/>.

- List all services available on the local network along with their addresses and ports while ignoring local ones:

`avahi-browse --all --resolve --ignore-local`

- List all domains:

`avahi-browse --browse-domains`

- Limit the search to a particular domain:

`avahi-browse --all --domain={{domain}}`
