# dnsmap 
## chatgpt 
The `dnsmap` command is a tool used for enumerating and mapping DNS (Domain Name System) networks. It is a command-line tool that can be used to conduct reconnaissance on a target by identifying DNS servers and their associated domains. The tool is essentially used to perform DNS brute-forcing, scanning, and enumeration.

Here are the various options and switches that can be used with `dnsmap`:

- `-r`: Use the specified DNS server as the resolver.
- `-i`: Use the specified input file instead of command line arguments.
- `-f`: Check all IP addresses in the specified range.
- `-z`: Check all IP addresses in the specified subnet.
- `-w`: Save results to a file.
- `-b`: Brute force subdomains by guessing names.
- `-c`: Only check the specified domain(s).
- `-p`: Use the specified UDP port for DNS resolution.
- `-v`: Set verbosity levels.

Some common usage examples of `dnsmap` include:

1. `dnsmap example.com` - This command will run a DNS enumeration scan on the domain "example.com" and list all observed subdomains.

2. `dnsmap -b subdomains.txt example.com` - The `-b` switch specifies brute-force subdomains by guessing names, using the words in the specified subdomain list. The command will then scan the domain "example.com" and match any observed subdomains with those in the list.

3. `dnsmap -f 192.168.0.1-255` - The `-f` switch specifies to check all IP addresses in the specified range. In this case, it will scan all hosts on the local network from "192.168.0.1-255" for open DNS servers.

Overall, `dnsmap` is a useful tool for sweep analysis and mapping of DNS networks to identify potential vulnerabilities and areas of interest for further analysis. 

## tldr 
 
> The dnsmap command scans a domain for common subdomains e.g. smtp.domain.org.
> More information: <https://github.com/resurrecting-open-source-projects/dnsmap>.

- Scan for subdomains using the internal wordlist:

`dnsmap {{example.com}}`

- Specify a list of subdomains to check for:

`dnsmap {{example.com}} -w {{path/to/wordlist.txt}}`

- Store results to a CSV file:

`dnsmap {{example.com}} -c {{path/to/file.csv}}`

- Ignore 2 IPs that are false positives (up to 5 possible):

`dnsmap {{example.com}} -i {{123.45.67.89,98.76.54.32}}`
