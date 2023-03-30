# acme.sh --dns 
## chatgpt 
The "acme.sh" command is a 3rd party client for the Let’s Encrypt CA (Certificate Authority) that allows users to obtain SSL/TLS (Secure Sockets Layer/Transport Layer Security) certificates.

The "--dns" option is one of the many options that can be used with acme.sh command. This option is used to automatically configure and use DNS APIs (Application Programming Interfaces) to complete domain validation for certificate issuance. 

When running the "acme.sh --dns" command, the ACME (Automated Certificate Management Environment) client will attempt to use an available DNS API and configure the required DNS records to validate the ownership of the domain for which the SSL/TLS certificate is being issued.

The use of DNS validation is necessary when the HTTP-based validation method (which involves placing a file on the server to verify domain ownership) can not be used. This can occur in situations where the user does not have direct control over the web server, or when the server is behind a firewall that does not allow external access.

Overall, the "acme.sh --dns" command is a powerful tool for automating the SSL/TLS certificate issuance process by leveraging DNS validation. 

## tldr 
 
> Use a DNS-01 challenge to issue a TLS certificate.
> More information: <https://github.com/acmesh-official/acme.sh/wiki>.

- Issue a certificate using an automatic DNS API mode:

`acme.sh --issue --dns {{gnd_gd}} --domain {{example.com}}`

- Issue a wildcard certificate (denoted by an asterisk) using an automatic DNS API mode:

`acme.sh --issue --dns {{dns_namesilo}} --domain {{example.com}} --domain {{*.example.com}}`

- Issue a certificate using a DNS alias mode:

`acme.sh --issue --dns {{dns_cf}} --domain {{example.com}} --challenge-alias {{alias-for-example-validation.com}}`

- Issue a certificate while disabling automatic Cloudflare / Google DNS polling after the DNS record is added by specifying a custom wait time in seconds:

`acme.sh --issue --dns {{dns_namecheap}} --domain {{example.com}} --dnssleep {{300}}`

- Issue a certificate using a manual DNS mode:

`acme.sh --issue --dns --domain {{example.com}} --yes-I-know-dns-manual-mode-enough-go-ahead-please`
