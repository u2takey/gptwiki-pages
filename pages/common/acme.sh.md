# acme.sh 
## chatgpt 
The `acme.sh` command is a script that is commonly used for issuing and managing SSL/TLS certificates from Let's Encrypt on Unix and Unix-like operating systems. It is a user-friendly and straightforward script that functions as a client for the Let's Encrypt certificate authority (CA).

The basic syntax for the `acme.sh` command is as follows:

```
acme.sh [OPTIONS] [COMMAND] [DOMAINS]
```

Here, `OPTIONS` refer to the additional parameters that may be necessary for the specific use case. `COMMAND` specifies the specific operation to be executed, such as `--install-cert` for installing the SSL/TLS certificate, `--renew` for renewing the certificate, and so on. `DOMAINS` are the fully qualified domain names (FQDNs) for which the certificate is being requested. 

Some of the commonly used options for the `acme.sh` command are:

- `-h, --help` : Displays the help menu
- `-d, --debug` : Enables debugging mode
- `-w, --webroot` : Specifies the root directory for the web server that will handle the HTTP-01 challenge
- `-k, --keylength` : Sets the length of the private key to be generated
- `-T, --staging` : Uses the Let's Encrypt staging server instead of the production server

The `acme.sh` command is highly versatile and can help automate the process of obtaining and renewing SSL/TLS certificates, ensuring that your web applications and websites are secure and properly encrypted. 

## tldr 
 
> Shell script implementing ACME client protocol, an alternative to certbot.
> See also `acme.sh dns`.
> More information: <https://github.com/acmesh-official/acme.sh>.

- Issue a certificate using webroot mode:

`acme.sh --issue --domain {{example.com}} --webroot {{/path/to/webroot}}`

- Issue a certificate for multiple domains using standalone mode using port 80:

`acme.sh --issue --standalone --domain {{example.com}} --domain {{www.example.com}}`

- Issue a certificate using standalone TLS mode using port 443:

`acme.sh --issue --alpn --domain {{example.com}}`

- Issue a certificate using a working Nginx configuration:

`acme.sh --issue --nginx --domain {{example.com}}`

- Issue a certificate using a working Apache configuration:

`acme.sh --issue --apache --domain {{example.com}}`

- Issue a wildcard (\*) certificate using an automatic DNS API mode:

`acme.sh --issue --dns {{dns_cf}} --domain {{*.example.com}}`

- Install certificate files into the specified locations (useful for automatic certificate renewal):

`acme.sh --install-cert -d {{example.com}} --key-file {{/path/to/example.com.key}} --fullchain-file {{/path/to/example.com.cer}} --reloadcmd {{"systemctl force-reload nginx"}}`
