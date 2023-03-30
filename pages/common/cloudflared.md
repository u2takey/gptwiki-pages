# cloudflared 
## chatgpt 
Cloudflared is a command line tool used to connect to Cloudflare's network. It is used to securely access web services that are hosted on the Cloudflare network using the Tunnel protocol.

The command cloudflared is used to start the tunneling process, where a secure and encrypted HTTPS tunnel is created between your device and the Cloudflare network. This allows you to connect to web services that are behind a firewall or on a private network.

To use cloudflared, you need to provide the command with a configuration file, which specifies the web service you want to connect to, the port, and the domain name. Once the configuration file is provided, the command will start the tunneling process and establish the encrypted connection.

Cloudflared is a powerful tool that provides enhanced security and improved access to web services hosted on the Cloudflare network. It is easy to use and is widely supported by many popular web services. 

## tldr 
 
> Command-line tool to create a persistent connection to the Cloudflare network.
> More information: <https://developers.cloudflare.com/argo-tunnel/>.

- Authenticate and associate the connection to a domain in the Cloudflare account:

`cloudflared tunnel login`

- Establish a tunnel to a host in Cloudflare from the local server:

`cloudflared tunnel --hostname {{hostname}} localhost:{{port_number}}`

- Establish a tunnel to a host in Cloudflare from the local server, without verifying the local server's certificate:

`cloudflared tunnel --hostname {{hostname}} localhost:{{port_number}} --no-tls-verify`

- Save logs to a file:

`cloudflared tunnel --hostname {{hostname}} http://localhost:{{port_number}} --loglevel {{panic|fatal|error|warn|info|debug}} --logfile {{path/to/file}}`

- Install cloudflared as a system service:

`cloudflared service install`
