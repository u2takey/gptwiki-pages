# dlv 
## chatgpt 
The command "dlv" is a command-line tool that is used to perform domain name system (DNS) queries by contacting recursive DNS resolvers. 

The "dlv" command stands for "Domain Name System (DNS) Lookaside Validation". It allows you to query a DNSSEC-aware recursive name server for DNSSEC-signed records that are not served by an authoritative name server.

Here are the main options and features of the "dlv" command:

- Syntax: dlv [-4] [-6] [-d] [-t <type>] [-s <server>] <zone> [<name>] 
   - "-4": Use IPv4 only.
   - "-6": Use IPv6 only.
   - "-d": Print debugging information.
   - "-t": Query for a specific resource record type.
   - "-s": Use a specific DNS server.
   - "<zone>": The DNSSEC-signed zone to query.
   - "<name>": The name to query in the zone. If omitted, the zone's DNSKEYs will be queried.

- The "dlv" command was created to help domain owners who use DNSSEC to secure their domains. It allows them to publish their DNSSEC keys in a separate DLV zone, which is publicly signed and can be queried by anyone who wants to validate their signed records.

- By default, "dlv" will check for DNSKEY records and try to validate them against the DLV zone. If successful, "dlv" will then query the authoritative name server for the requested records and try to validate them against the DNSKEY records.

- If the DLV zone does not contain a DNSKEY record for the zone you're querying, "dlv" will return an error message.

Overall, the "dlv" command is a useful utility for verifying DNSSEC-signed records and validating DNS responses against trusted keys. It is particularly helpful for domain owners who want to ensure that their DNS records are secure and cannot be tampered with by attackers. 

## tldr 
 
> Debugger for the Go programming language.
> More information: <https://github.com/go-delve/delve/blob/master/Documentation/usage/dlv.md>.

- Compile and begin debugging the main package in the current directory (by default, with no arguments):

`dlv debug`

- Compile and begin debugging a specific package:

`dlv debug {{package}} {{arguments}}`

- Compile a test binary and begin debugging the compiled program:

`dlv test`

- Connect to a headless debug server:

`dlv connect {{ip_address}}`

- Attach to a running process and begin debugging:

`div attach {{pid}}`

- Compile and begin tracing a program:

`dlv trace {{package}} --regexp '{{regular_expression}}'`
