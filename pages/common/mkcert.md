# mkcert 
## chatgpt 
The "mkcert" command, short for "make certificate," is a command-line tool used for generating trusted TLS certificates for local development or testing purposes. This allows developers to set up secure HTTPS connections between their local development environment and their web application or API without having to rely on self-signed certificates that can generate warnings or errors in web browsers. The mkcert tool uses the root certificate authority on the local machine to sign the generated certificates, which makes them automatically trusted by the operating system and any applications or web browsers running on it. 

The mkcert command has various commands and options, some of which include:

- "mkcert -install": This command installs the root certificate authority in the system's trust store, which enables the generated certificates to be trusted by the operating system and applications.

- "mkcert example.com": This command generates a TLS certificate for the example.com domain, which can be used for secure connection between a local server and a web browser or API client.

- "mkcert -key-file key.pem -cert-file cert.pem example.com": This command generates the TLS certificate with a custom name for the key and certificate files, which can be specified with the -key-file and -cert-file options respectively.

Overall, the mkcert command provides a simple and secure way to generate trusted TLS certificates for local development, which helps to ensure that the web application or API being developed operates as expected in a secure HTTPS environment. 

## tldr 
 
> Tool for making locally-trusted development certificates.
> More information: <https://github.com/FiloSottile/mkcert>.

- Install the local CA in the system trust store:

`mkcert -install`

- Generate certificate and private key for a given domain:

`mkcert {{example.org}}`

- Generate certificate and private key for multiple domains:

`mkcert {{example.org}} {{myapp.dev}} {{127.0.0.1}}`

- Generate wildcard certificate and private key for a given domain and its subdomains:

`mkcert "{{*.example.it}}"`

- Uninstall the local CA:

`mkcert -uninstall`
