# kdig 
## chatgpt 
The `kdig` command is a utility for performing DNS queries from a command-line interface. It is similar to other DNS query tools like `nslookup` and `dig`, but offers some additional features and options.

Here are some details on how to use `kdig`:

Syntax:
```
kdig [options] [name] [type] [class]
```

Options:
- `-h`: Display help information.
- `-v`: Verbose output, including additional information about the response.
- `-x`: Reverse DNS lookup, where the IP address is provided instead of the domain name.
- `-t [type]`: Specify the DNS record type, such as A, NS, MX, etc.
- `-c [class]`: Specify the DNS class, typically IN for Internet.
- `-p [port]`: Specify the UDP or TCP port to query, default is 53.
- `-d [domain]`: Set the search domain to be appended to queries if no domain name is given.
- `-y [keyname]:[keyvalue]`: Provide a TSIG key for authenticated queries.
- `-a [server]`: Use alternate DNS server for the query.
- `-f [filename]`: Read queries from a file rather than from the command line.

Examples:

1. Simple query for an A record:
```
kdig example.com A
```
This will perform a DNS query for the A record of example.com.

2. Reverse lookup for an IP address:
```
kdig -x 8.8.8.8
```
This will perform a reverse DNS lookup for the IP address 8.8.8.8 (which is the Google Public DNS).

3. Query for a specific DNS record type:
```
kdig google.com MX
```
This will perform a DNS query for the MX (mail exchange) records of google.com.

Overall, `kdig` is a powerful and flexible utility for performing DNS queries from the command line, with many options for customizing the queries and obtaining detailed output. 

## tldr 
 
> Advanced DNS lookup utility.
> More information: <https://www.knot-dns.cz/docs/latest/html/man_kdig.html>.

- Lookup the IP(s) associated with a hostname (A records):

`kdig {{example.com}}`

- Specify a specific DNS server to query (e.g. Google DNS):

`kdig {{example.com}} @{{8.8.8.8}}`

- Query a specific DNS record type associated with a given domain name:

`kdig {{example.com}} {{A|AAAA|NS|SOA|DNSKEY|ANY}}`

- Lookup the IP(s) associated with a hostname (A records) using DNS over TLS (DoT):

`kdig -d @{{8.8.8.8}} +tls-ca +tls-host={{dns.google}} {{example.com}}`

- Lookup the IP(s) associated with a hostname (A records) using DNS over HTTPS (DoH):

`kdig -d @{{1.1.1.1}} +https +tls-hostname={{1dot1dot1dot1.cloudflare-dns.com}} {{example.com}}`
