# dnsrecon 
## chatgpt 
The 'dnsrecon' command is used for reconnaissance of Domain Name System (DNS) infrastructure. This command is used to identify and locate all DNS servers, subdomains, and other related services used by a domain.

Some of the actions performed by the 'dnsrecon' command are:

1. DNS zone transfer (AXFR) testing: Zone transfer is a mechanism used by DNS servers to replicate their database information to other servers. The 'dnsrecon' command checks if the target domain allows zone transfer.

2. Subdomain enumeration: 'dnsrecon' command can be used to enumerate all the subdomains of a particular domain name. The tool uses various methods such as brute force, dictionary attacks, and other techniques to detect all subdomains.

3. Reverse DNS lookup: The 'dnsrecon' command can be used to reverse lookup IP addresses and map them back to domain names.

4. DNS cache snooping: This is a technique used to identify DNS entries that are stored in the cache of the DNS server. The 'dnsrecon' command can be used to snoop through the DNS cache and get information about previous DNS queries.

Overall, the 'dnsrecon' command is a powerful tool for reconnaissance of DNS infrastructure, which can help in detecting potential vulnerabilities or attack vectors for a domain. It is commonly used by cybersecurity professionals and ethical hackers as a part of their reconnaissance phase. 

## tldr 
 
> DNS enumeration tool.
> More information: <https://github.com/darkoperator/dnsrecon>.

- Scan a domain and save the results to a SQLite database:

`dnsrecon --domain {{example.com}} --db {{path/to/database.sqlite}}`

- Scan a domain, specifying the nameserver and performing a zone transfer:

`dnsrecon --domain {{example.com}} --name_server {{nameserver.example.com}} --type axfr`

- Scan a domain, using a brute-force attack and a dictionary of subdomains and hostnames:

`dnsrecon --domain {{example.com}} --dictionary {{path/to/dictionary.txt}} --type brt`

- Scan a domain, performing a reverse lookup of IP ranges from the SPF record and saving the results to a JSON file:

`dnsrecon --domain {{example.com}} -s --json`

- Scan a domain, performing a Google enumeration and saving the results to a CSV file:

`dnsrecon --domain {{example.com}} -g --csv`

- Scan a domain, performing DNS cache snooping:

`dnsrecon --domain {{example.com}} --type snoop --name_server {{nameserver.example.com}} --dictionary {{path/to/dictionary.txt}}`

- Scan a domain, performing zone walking:

`dnsrecon --domain {{example.com}} --type zonewalk`
