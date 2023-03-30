# cockpit-tls 
## chatgpt 
Cockpit-tls is a command-line tool for managing Transport Layer Security (TLS) certificates used by the Cockpit web-based administration tool. 

The command is used to generate a self-signed TLS certificate for use with Cockpit. TLS is a cryptographic protocol used to establish secure connections between web servers and clients.

When the command is executed, it generates a new self-signed TLS certificate with default settings, including the Common Name (CN) of the signed certificate, and the expiry date. If preferred, specific settings for the certificate can be set, such as the CN name, organization name, and email address.

Overall, the cockpit-tls command is an essential tool for managing secure communication between web servers and clients with the Cockpit administration tool. 

## tldr 
 
> TLS terminating HTTP proxy to encrypt traffic between a client and `cockpit-ws`.
> More information: <https://cockpit-project.org/guide/latest/cockpit-tls.8.html>.

- Serve HTTP requests to a specific port instead of port `9090`:

`cockpit-tls --port {{port}}`

- Display help:

`cockpit-tls --help`
