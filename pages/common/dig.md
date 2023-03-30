# dig 
## chatgpt 
"dig" is a command-line tool in Linux and other Unix-based operating systems that is used to query DNS servers to get information about domain names such as IP addresses, name servers, and other DNS records. 

The syntax for the command is: 

```
dig [domain name] [options]
```

Here, "[domain name]" refers to any valid domain name such as google.com or yahoo.co.uk, and "[options]" are any other parameters that may be used to modify the behavior of the command. Some of the commonly used options include:

- "+short": This option returns a shortened output, displaying only the IP address(es) associated with the domain name, without any additional information.
- "+trace": This option performs a trace of the query, showing the complete path of DNS servers that are queried along the way.
- "+recurse": This option forces the DNS server to perform a recursive query, which means that it will continue to query other DNS servers until it finds the information it needs.

In addition to these options, there are many other parameters that can be used with the "dig" command, such as setting the query type (e.g. A, MX, CNAME), setting the DNS server to query, and specifying a specific port to use for the query. The output of the "dig" command provides useful information for network administrators and webmasters, as it can help in troubleshooting DNS issues and verifying DNS configurations. 

## tldr 
 
> DNS lookup utility.
> More information: <https://manned.org/dig>.

- Lookup the IP(s) associated with a hostname (A records):

`dig +short {{example.com}}`

- Get a detailed answer for a given domain (A records):

`dig +noall +answer {{example.com}}`

- Query a specific DNS record type associated with a given domain name:

`dig +short {{example.com}} {{A|MX|TXT|CNAME|NS}}`

- Get all types of records for a given domain name:

`dig {{example.com}} ANY`

- Specify an alternate DNS server to query:

`dig @{{8.8.8.8}} {{example.com}}`

- Perform a reverse DNS lookup on an IP address (PTR record):

`dig -x {{8.8.8.8}}`

- Find authoritative name servers for the zone and display SOA records:

`dig +nssearch {{example.com}}`

- Perform iterative queries and display the entire trace path to resolve a domain name:

`dig +trace {{example.com}}`
