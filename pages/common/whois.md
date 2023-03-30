# whois 
## chatgpt 
The `whois` command is used to obtain information about domain names, IP addresses and Autonomous System (AS) numbers registered with various organizations such as ICANN, RIPE, ARIN, APNIC, etc. The command sends a query to a specific whois server and retrieves information about the domain or IP address.

Syntax:
```
whois [options] <query>
```

The options can include the following:
- `-h`: specifies the whois server to query
- `-p`: specifies the port number to use
- `-v`: displays the version of whois being used
- `-i`: displays more detailed information about the domain

The query can be a domain name or an IP address.

When the `whois` command is run with a domain name as the query, it returns information about the domain name such as the registrar, nameservers, creation and expiration date, etc. 

For example, `whois google.com` would return information about the Google domain name.

When the `whois` command is run with an IP address as the query, it returns information about the organization that owns the IP address such as the network name, address range, and contact information.

For example, `whois 216.58.194.174` would return information about one of Google's IP addresses. 

## tldr 
 
> Command-line client for the WHOIS (RFC 3912) protocol.
> More information: <https://github.com/rfc1036/whois>.

- Get information about a domain name:

`whois {{example.com}}`

- Get information about an IP address:

`whois {{8.8.8.8}}`

- Get abuse contact for an IP address:

`whois -b {{8.8.8.8}}`
