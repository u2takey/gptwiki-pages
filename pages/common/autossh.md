# autossh 
## chatgpt 
The `autossh` command is a program that automatically restarts an SSH tunnel if it dies or is disconnected. It is designed to help maintain persistent and stable connections over unreliable networks or during system reboots.

The `autossh` command works by periodically checking the SSH tunnel to make sure it is still active. If the tunnel is no longer active, `autossh` will automatically restart the tunnel using the same settings as before. In addition, `autossh` can also keep the SSH session alive by sending keepalive packets to the remote server, preventing the connection from timing out due to inactivity.

Here is an example of how to use the `autossh` command:

```
autossh -M 0 -N -o "ServerAliveInterval 30" -o "ServerAliveCountMax 3" -i /path/to/private/key -L 8080:localhost:80 user@remotehost
```

In this example, we are using several options to configure the `autossh` command:

- `-M 0` disables the monitoring port feature, which is not needed in this case.
- `-N` tells `autossh` not to execute any remote commands, but instead to just establish the SSH tunnel.
- `-o "ServerAliveInterval 30"` tells `autossh` to send a keepalive packet to the remote server every 30 seconds.
- `-o "ServerAliveCountMax 3"` tells `autossh` to terminate the connection if it doesn't receive a response after 3 keepalive packets.
- `-i /path/to/private/key` specifies the location of the private key used for authentication.
- `-L 8080:localhost:80` sets up a tunnel that forwards traffic from port 8080 on the local machine to port 80 on the remote machine.
- `user@remotehost` specifies the remote host to connect to, along with the username to use for authentication.

Overall, `autossh` is a very useful tool for maintaining stable SSH connections over unreliable networks. By automatically restarting the SSH tunnel and sending keepalive packets, `autossh` can help ensure that your connections stay up even in challenging conditions. 

## tldr 
 
> Run, monitor and restart SSH connections.
> Auto-reconnects to keep port forwarding tunnels up. Accepts all `ssh` flags.
> More information: <https://www.harding.motd.ca/autossh>.

- Start an SSH session, restarting when a monitoring port fails to return data:

`autossh -M {{monitor_port}} "{{ssh_command}}"`

- Forward a local port to a remote one, restarting when necessary:

`autossh -M {{monitor_port}} -L {{local_port}}:localhost:{{remote_port}} {{user}}@{{host}}`

- Fork `autossh` into the background before executing `ssh` and don't open a remote shell:

`autossh -f -M {{monitor_port}} -N "{{ssh_command}}"`

- Run in the background, with no monitoring port, and instead send SSH keep-alive packets every 10 seconds to detect failure:

`autossh -f -M 0 -N -o "ServerAliveInterval 10" -o "ServerAliveCountMax 3" "{{ssh_command}}"`

- Run in the background, with no monitoring port and no remote shell, exiting if the port forward fails:

`autossh -f -M 0 -N -o "ServerAliveInterval 10" -o "ServerAliveCountMax 3" -o ExitOnForwardFailure=yes -L {{local_port}}:localhost:{{remote_port}} {{user}}@{{host}}`

- Run in the background, logging `autossh` debug output and `ssh` verbose output to files:

`AUTOSSH_DEBUG=1 AUTOSSH_LOGFILE={{path/to/autossh_log_file.log}} autossh -f -M {{monitor_port}} -v -E {{path/to/ssh_log_file.log}} {{ssh_command}}`
