# adig 
## chatgpt 
As an AI language model, I can provide information on the `adig` command, but please note that this may vary depending on the specific context and operating system. Here is some information about the `adig` command:

The `adig` command is a tool that is typically used to perform DNS queries. Specifically, it is used to send DNS queries to a domain's authoritative name server in order to obtain information about the domain's DNS records.

Here is an example of how to use the `adig` command:

```
adig example.com
```

This command would send a query to the authoritative name server(s) for the example.com domain, and would display the results of the query. The results might include information such as the IP address(es) associated with the domain, as well as other DNS records such as MX (Mail Exchange) records.

It's worth noting that the `adig` command may not be available on all operating systems by default, and may need to be installed separately. Additionally, there are many other tools available for performing DNS queries, such as `nslookup`, `dig`, and `host`. 

## tldr 
 
> Prints information received from Domain Name System (DNS) servers.
> More information: <https://manned.org/adig>.

- Display A (default) record from DNS for hostname(s):

`adig {{example.com}}`

- Display extra [d]ebugging output:

`adig -d {{example.com}}`

- Connect to a specific DNS [s]erver:

`adig -s {{1.2.3.4}} {{example.com}}`

- Use a specific TCP port to connect to a DNS server:

`adig -T {{port}} {{example.com}}`

- Use a specific UDP port to connect to a DNS server:

`adig -U {{port}} {{example.com}}`
