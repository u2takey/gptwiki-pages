# mosh 
## chatgpt 
Mosh is a command-line tool that stands for Mobile Shell. It is designed to allow remote connectivity to a command-line session on a remote server through a secure shell connection on unreliable network connections such as high latency, intermittent connectivity, or a low bandwidth.

Mosh is designed to be a replacement for SSH, which can have issues when dealing with unreliable network connections. Mosh addresses these issues by using a combination of UDP and SSH to establish a secure connection between the client and the server.

The syntax for using the mosh command is:

```
mosh [options] username@host [command]
```

Where `[options]` are various command options that can be used with the mosh command to customize the user experience, `[username]` is the username you want to use to log in to the remote server, `[host]` is the IP address or hostname of the remote server, and `[command]` is an optional command that you want to run on the remote server.

Some of the commonly used options with mosh command are:

- `-p`: specifies the port to connect to on the remote server
- `-l`: specifies the local address to bind to
- `-4`: forces the use of IPv4 addresses
- `-6`: forces the use of IPv6 addresses
- `-v`: enables verbose mode

Overall, the mosh command is a valuable tool for anyone who wants to have a reliable and secure connection to a remote server, especially in situations where the network connection is unreliable. 

## tldr 
 
> Mobile Shell (`mosh`) is a robust and responsive replacement for SSH.
> `mosh` persists connections to remote servers while roaming between networks.
> More information: <https://mosh.org>.

- Connect to a remote server:

`mosh {{username}}@{{remote_host}}`

- Connect to a remote server with a specific identity (private key):

`mosh --ssh="ssh -i {{path/to/key_file}}" {{username}}@{{remote_host}}`

- Connect to a remote server using a specific port:

`mosh --ssh="ssh -p {{2222}}" {{username}}@{{remote_host}}`

- Run a command on a remote server:

`mosh {{remote_host}} -- {{command -with -flags}}`

- Select Mosh UDP port (useful when `{{remote_host}}` is behind a NAT):

`mosh -p {{124}} {{username}}@{{remote_host}}`

- Usage when `mosh-server` binary is outside standard path:

`mosh --server={{path/to/bin/}}mosh-server {{remote_host}}`
