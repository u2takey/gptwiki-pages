# openssl s_client 
## chatgpt 
The `openssl s_client` command is a command line tool that allows users to initiate a secure SSL/TLS connection to a server and then communicate with it. Here is a detailed explanation of each component of the command:

- `openssl`: This is the command for the OpenSSL tool, an open-source encryption library that provides functionality for secure communication over networks.
- `s_client`: This is a sub-command within the OpenSSL tool that initiates an SSL/TLS connection to a server and acts as a client to communicate with it.

When you enter the command `openssl s_client` followed by additional options and arguments, here are some of the things that this command does:

- Initiate an SSL/TLS handshake with the server, which involves various steps of negotiation and authentication to establish a secure connection.
- Verify the server's SSL/TLS certificate to ensure that it is valid and trustworthy.
- Establish a secure connection between the local system and the remote server, so that all subsequent communication is encrypted and protected against unauthorized access.
- Show information about the server's SSL/TLS configuration, such as the encryption protocols and cipher suites that are supported.
- Provide a command prompt where you can send commands or data to the server and receive responses or output.

Some common options that you might use with `openssl s_client` include:

- `-connect <host>:<port>`: Specify the hostname and port number of the server that you want to connect to.
- `-cert <certificate>` and `-key <private key>`: Provide a client-side SSL/TLS certificate and private key for authentication, if required by the server.
- `-CAfile <certificate authority file>` and `-verify <depth>`: Set up certificate chain validation to ensure that the server's certificate is trusted and valid.
- `-showcerts` and `-servername <hostname>`: Display information about the server's SSL/TLS certificate, and specify the hostname to send in the SNI (Server Name Indication) extension when connecting to a virtual host. 

## tldr 
 
> OpenSSL command to create TLS client connections.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-s_client.html>.

- Display the start and expiry dates for a domain's certificate:

`openssl s_client -connect {{host}}:{{port}} 2>/dev/null | openssl x509 -noout -dates`

- Display the certificate presented by an SSL/TLS server:

`openssl s_client -connect {{host}}:{{port}} </dev/null`

- Set the Server Name Indicator (SNI) when connecting to the SSL/TLS server:

`openssl s_client -connect {{host}}:{{port}} -servername {{hostname}}`

- Display the complete certificate chain of an HTTPS server:

`openssl s_client -connect {{host}}:443 -showcerts </dev/null`
