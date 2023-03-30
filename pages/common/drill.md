# drill 
## chatgpt 
The 'drill' command is a command-line tool that is used for performing advanced DNS queries against DNS servers. It is commonly used for DNS troubleshooting, debugging, and network testing. Here are some details about the drill command:

Syntax:

drill [options] domain

Options:

1. -a - List all records for a domain.
2. -C - Print the output in a CSV (comma-separated value) format.
3. -c - Specify the number of retries in case of a timeout.
4. -D - Enable debugging output.
5. -f - Specify the input file to read the queries from.
6. -h - Print out the help message.
7. -m - Specify the maximum number of retries.
8. -N - Disable TCP queries.
9. -o - Specify the output file.
10. -p - Specify the port number for the DNS server.
11. -q - Specify the query type (A, AAAA, CNAME, etc.).
12. -r - Specify the record type (SOA, NS, MX, etc.).
13. -S - Use TCP for all queries.
14. -s - Specify the DNS server to query.
15. -t - Specify the timeout in seconds.

Uses:

1. To test the DNS server's response time.
2. To check for DNS server configuration issues.
3. To find out the authoritative name server for a domain.
4. To find out a DNS record's TTL (time to live) value.
5. To perform name server delegation testing.
6. To perform DNSSEC (DNS Security Extensions) and DNS query authentication.
7. To perform reverse DNS lookup testing.

Overall, the drill command is a powerful tool that is used for DNS testing and troubleshooting. It can provide a detailed, granular view of DNS server responses and can help network administrators identify and resolve DNS-related issues. 

## tldr 
 
> Perform various DNS queries.
> More information: <https://manned.org/drill>.

- Lookup the IP(s) associated with a hostname (A records):

`drill {{example.com}}`

- Lookup the mail server(s) associated with a given domain name (MX record):

`drill mx {{example.com}}`

- Get all types of records for a given domain name:

`drill any {{example.com}}`

- Specify an alternate DNS server to query:

`drill {{example.com}} @{{8.8.8.8}}`

- Perform a reverse DNS lookup on an IP address (PTR record):

`drill -x {{8.8.8.8}}`

- Perform DNSSEC trace from root servers down to a domain name:

`drill -TD {{example.com}}`

- Show DNSKEY record(s) for a domain name:

`drill -s dnskey {{example.com}}`
