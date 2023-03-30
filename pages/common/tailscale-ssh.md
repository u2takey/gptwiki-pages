# tailscale ssh 
## chatgpt 
`tailscale ssh` is a command used to connect to a remote machine or server over SSH (Secure Shell) that is connected to you through the Tailscale VPN network. Once connected, you can securely navigate the remote machine's file system, run commands, and perform other tasks. 

Here is a breakdown of the components of the `tailscale ssh` command:

- `tailscale`: This command is a part of the Tailscale VPN application, which is a mesh VPN (Virtual Private Network) solution that allows you to securely connect devices and networks across different locations. 
- `ssh`: This is the command used to establish a secure shell connection to a remote machine or server. 

To use the `tailscale ssh` command, you need to have the Tailscale VPN running on both the local and remote machines. Once connected to the Tailscale VPN network, you can run the `tailscale ssh` command to initiate an SSH connection to a remote machine using the following syntax:

```tailscale ssh [user@]host[:port]```

- `user`: This is the username that you use to log in to the remote machine. If you don't specify a username, the default username will be used.
- `host`: This is the hostname or IP address of the remote machine that you want to connect to.
- `port`: This is the SSH port that the remote machine is listening on. If you don't specify a port, the default SSH port (22) will be used.

Once you have entered the command with the appropriate parameters, you will be prompted for the login credentials for the remote machine. Once authenticated, you can begin running commands on the remote machine through the secure shell connection. 

## tldr 
 
> SSH to a Tailscale machine (Linux Only).
> More information: <https://tailscale.com/kb/1193/tailscale-ssh>.

- Advertise/Disable SSH on the host:

`sudo tailscale up --ssh={{true|false}}`

- SSH to a specific host which has Tailscale-SSH enabled:

`tailscale ssh {{username}}@{{host}}`
