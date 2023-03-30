# vpnc 
## chatgpt 
The vpnc command is a Linux command used for configuring client-side virtual private network (VPN) connections using the Cisco VPN protocol. Here's a description of the command and its options:

`vpnc` - This is the main command that launches the vpnc client.

Options:

- `-s` or `--no-detach`: Runs vpnc in the foreground and displays error messages on the screen.
- `-c <filename>` or `--config <filename>`: Specifies the configuration file to use. If no configuration file is specified, vpnc will use the default /etc/vpnc/default.conf file.
- `-u <username>` or `--username <username>`: Specifies the username to use for the VPN connection.
- `-d <domain>` or `--domain <domain>`: Specifies the Windows domain name to use. This is only needed for Windows-based VPN servers.
- `-r <group>` or `--group <group>`: Specifies the group name to use for the VPN connection.
- `-t <timeout>` or `--timeout <timeout>`: Specifies the number of seconds to wait for a response from the VPN server before timing out.
- `-p <password>` or `--password <password>`: Specifies the password to use for the VPN connection. WARNING: Using this option may expose your password to others!
- `-k <key>` or `--psk <key>`: Specifies the pre-shared key to use for the VPN connection. This is only needed for L2TP/IPSec VPN connections.

Overall, vpnc is a powerful and versatile command-line tool for configuring VPN connections on Linux systems. However, you should carefully read the documentation and instructions before using it to ensure that you configure your VPN connection correctly and securely. 

## tldr 
 
> A VPN client for the Cisco 3000 VPN Concentrator.
> More information: <https://manned.org/vpnc>.

- Connect with a defined configuration file:

`sudo vpnc {{config_file}}`

- Terminate the previously created connection:

`sudo vpnc-disconnect`
