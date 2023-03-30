# amass 
## chatgpt 
Amass is a command-line tool used for subdomain enumeration and information gathering. It is available for different operating systems such as Windows, Linux, and macOS. The tool is designed to help users find domains and subdomains related to a target domain or IP address, search for open ports, and identify potential vulnerabilities.

The amass command can be used with various options and parameters to allow users to search for subdomains in different ways. Some of the most commonly used options include:

- amass enum: This option allows the user to enumerate subdomains using various techniques such as DNS brute-forcing, web scraping, zone transfers, and reverse DNS queries.

- amass intel: This option helps in collecting additional data related to the target domain or IP address, such as IP addresses, WHOIS details, and SSL/TLS certificates.

- amass enum --passive: This option is used for passive reconnaissance, which uses public data sources to collect information about the target without sending any requests or queries.

- amass enum --active: This option involves active reconnaissance, which involves sending requests or queries to the target domain or IP address to collect information.

- amass track: This option allows users to track changes made to the target domain, such as new subdomains or DNS record changes.

Overall, the amass command is a useful tool for network administrators, security researchers, and penetration testers who need to gather information about a target domain and identify potential vulnerabilities. 

## tldr 
 
> In-depth Attack Surface Mapping and Asset Discovery tool.
> Some subcommands such as `amass db` have their own usage documentation.
> More information: <https://github.com/OWASP/Amass>.

- Execute an Amass subcommand:

`amass {{subcommand}}`

- Show general help:

`amass -help`

- Show help on an Amass subcommand (like `intel`, `enum`, etc.):

`amass -help {{subcommand}}`

- Display version:

`amass -version`
