# host 
## chatgpt 
The `host` command is a command-line utility tool used to get information about a hostname or an IP address. It is available on most operating systems, including Unix, Linux, and macOS. 

The basic syntax for using the `host` command is:

```
host hostname/IP_address
```

When this command is run, it looks up the IP address of the host name or the hostname of an IP address and returns the relevant information. The output includes the fully qualified domain name (FQDN), the IP address associated with the hostname, and the type of record being queried (i.e., A, PTR, MX, etc.).

For example, the following command will return the IP address and FQDN for the hostname "google.com":

```
host google.com
```

The output will be something like:

```
google.com has address 172.217.167.174
google.com has IPv6 address 2607:f8b0:4002:809::200e
google.com mail is handled by 10 aspmx.l.google.com.
google.com mail is handled by 20 alt1.aspmx.l.google.com.
google.com mail is handled by 20 alt2.aspmx.l.google.com.
google.com mail is handled by 30 aspmx2.googlemail.com.
google.com mail is handled by 30 aspmx3.googlemail.com.
google.com mail is handled by 30 aspmx4.googlemail.com.
google.com mail is handled by 30 aspmx5.googlemail.com.
```

This output shows that for the hostname "google.com," there are several email servers (MX records) associated with it, along with two IPv4 and one IPv6 address (A and AAAA records). 

Overall, the `host` command is a useful tool when looking up hostnames and IP addresses and retrieving DNS information. 

## tldr 
 
> Lookup Domain Name Server.
> More information: <https://manned.org/host>.

- Lookup A, AAAA, and MX records of a domain:

`host {{domain}}`

- Lookup a field (CNAME, TXT,...) of a domain:

`host -t {{field}} {{domain}}`

- Reverse lookup an IP:

`host {{ip_address}}`

- Specify an alternate DNS server to query:

`host {{domain}} {{8.8.8.8}}`
