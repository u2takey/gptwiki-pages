# nslookup 
## chatgpt 
The nslookup command is a network diagnostic tool used to obtain information about a domain name or an IP address. It is a command line tool that is available on almost all operating systems including Windows, Unix, and Linux.

When you run the nslookup command, it first queries the default DNS server configured on your system to resolve the IP address or domain name. The results include the IP address or domain name of the requested resource, as well as other information such as the DNS server, its IP address, the name of the authoritative name server, and the domain name associated with the IP address.

To use nslookup, open the command prompt or terminal on your operating system and type "nslookup". You can then enter the domain name or IP address you wish to query. For example, to obtain information about the domain "google.com", enter "nslookup google.com". If you want to obtain information about an IP address, enter "nslookup <ip_address>".

Overall, the nslookup command is a useful network diagnostic tool that is used by IT professionals to troubleshoot DNS server issues and to obtain information about a domain or IP address. 

## tldr 
 
> Query name server(s) for various domain records.
> More information: <https://manned.org/nslookup>.

- Query your system's default name server for an IP address (A record) of the domain:

`nslookup {{example.com}}`

- Query a given name server for a NS record of the domain:

`nslookup -type=NS {{example.com}} {{8.8.8.8}}`

- Query for a reverse lookup (PTR record) of an IP address:

`nslookup -type=PTR {{54.240.162.118}}`

- Query for ANY available records using TCP protocol:

`nslookup -vc -type=ANY {{example.com}} `

- Query a given name server for the whole zone file (zone transfer) of the domain using TCP protocol:

`nslookup -vc -type=AXFR {{example.com}} {{name_server}}`

- Query for a mail server (MX record) of the domain, showing details of the transaction:

`nslookup -type=MX -debug {{example.com}}`

- Query a given name server on a specific port number for a TXT record of the domain:

`nslookup -port={{port_number}} -type=TXT {{example.com}} {{name_server}}`
