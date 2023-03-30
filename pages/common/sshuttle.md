# sshuttle 
## chatgpt 
SSHuttle is a command-line tool that allows you to create a VPN-like connection to a remote server, using only SSH. It can be used for secure browsing and accessing remote networks.

Here's a breakdown of the command:

```
sshuttle [options] server
```

- `sshuttle`: This is the command to initiate the VPN-like connection using SSH.
- `[options]`: These are the different flags and options that you can use with the `sshuttle` command. For example, you can specify the port number to use for the SSH connection, or which remote networks you want to access.
- `server`: This is the remote server that you want to connect to. You'll need to have SSH access to this server in order to use `sshuttle`.

Once you run the `sshuttle` command, it will set up a VPN-like connection between your local machine and the remote server. All traffic between your local machine and the remote server will be encrypted, and you'll be able to access remote networks and resources as if you were directly connected to them. 

## tldr 
 
> Transparent proxy server that tunnels traffic over an SSH connection.
> Doesn't require root or any special setup on the remote SSH server, though root access on the local machine is prompted for.
> More information: <https://manned.org/sshuttle>.

- Forward all IPv4 TCP traffic via a remote SSH server:

`sshuttle --remote={{username}}@{{sshserver}} {{0.0.0.0/0}}`

- Also forward all DNS traffic to the server's default DNS resolver:

`sshuttle --dns --remote={{username}}@{{sshserver}} {{0.0.0.0/0}}`

- Forward all traffic except that which is bound for a specific subnet:

`sshuttle --remote={{username}}@{{sshserver}} {{0.0.0.0/0}} --exclude {{192.168.0.1/24}}`

- Use the tproxy method to forward all IPv4 and IPv6 traffic:

`sshuttle --method=tproxy --remote={{username}}@{{sshserver}} {{0.0.0.0/0}} {{::/0}} --exclude={{your_local_ip_address}} --exclude={{ssh_server_ip_address}}`
