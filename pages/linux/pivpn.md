# pivpn 
## chatgpt 
The "pivpn" command is used to install and manage a Virtual Private Network (VPN) on a Raspberry Pi device running the Raspbian operating system. 

Here are some actions that can be performed using the pivpn command:

1. Install a VPN: With the "pivpn add" command, you can install a VPN on your Raspberry Pi device. The tool handles most of the configuration process for you and you can choose the type of VPN you want to set up.

2. Manage a VPN: You can manage your VPN using various commands such as "pivpn revoke" to remove a client, "pivpn list" to view a list of all clients that have access to the VPN, and "pivpn debug" to access the logs of your VPN.

3. Update a VPN: You can use the "pivpn update" command to update your VPN to the latest version if any updates are available.

4. Generate a Diffie-Hellman key: You can use the "pivpn dhparam" command to generate a Diffie-Hellman key for your VPN. This key is used to establish a secure connection between the client and the server.

5. Uninstall a VPN: You can use the "pivpn uninstall" command to completely remove the VPN from your Raspberry Pi device.

In summary, the pivpn command is a tool that simplifies the process of installing and managing a VPN on Raspberry Pi devices. 

## tldr 
 
> Easy security-hardened OpenVPN setup and manager.
> Originally designed for the Raspberry Pi, but works on other Linux devices too.
> More information: <http://www.pivpn.io/>.

- Add a new client device:

`sudo pivpn add`

- List all client devices:

`sudo pivpn list`

- List currently connected devices and their statistics:

`sudo pivpn clients`

- Revoke a previously authenticated device:

`sudo pivpn revoke`

- Uninstall PiVPN:

`sudo pivpn uninstall`
