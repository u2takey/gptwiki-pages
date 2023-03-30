# ngrok 
## chatgpt 
Ngrok is a command-line tool used to create secure tunnels to localhost, allowing external access to a local network. It is commonly used for testing and debugging web applications or APIs, and is particularly useful when working with webhooks or other tools that require external access to a local server.

To use ngrok, you first need to download and install the tool on your machine. Once installed, you can run the ngrok command followed by the port number you want to tunnel (e.g. ngrok 8000).

Ngrok will then generate a unique public URL that you can share with others, allowing them to access your local server from outside your network. This URL is typically in the format "https://<random-string>.ngrok.io".

When you start ngrok, it opens a secure tunnel between your local server and the ngrok servers, using a secure SSL/TLS connection. This ensures that traffic between your server and the ngrok servers is encrypted, preventing any third-party from intercepting or modifying the traffic.

Overall, ngrok is a powerful tool that simplifies the process of creating secure tunnels to localhost. It allows developers to test and debug web applications or APIs in a safe and controlled environment, without the need for complex network configurations. 

## tldr 
 
> Reverse proxy that creates a secure tunnel from a public endpoint to a locally running web service.
> More information: <https://ngrok.com>.

- Expose a local HTTP service on a given port:

`ngrok http {{80}}`

- Expose a local HTTP service on a specific host:

`ngrok http {{foo.dev}}:{{80}}`

- Expose a local HTTPS server:

`ngrok http https://localhost`

- Expose TCP traffic on a given port:

`ngrok tcp {{22}}`

- Expose TLS traffic for a specific host and port:

`ngrok tls -hostname={{foo.com}} {{443}}`
