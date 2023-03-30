# nmcli device 
## chatgpt 
The `nmcli device` command is used to manage network devices in Linux systems. 

The `nmcli` command stands for Network Manager Command Line interface, which is a tool used to interact with the Network Manager on a Linux system. 

The `device` argument is used to specify that we want to manage network devices specifically. 

When we run the `nmcli device` command, it will output a list of all the network devices that are available on the system. This includes both physical and virtual devices. For example, Ethernet adapters, WiFi adapters, and virtual devices like VPN connections. 

From the output of the `nmcli device` command, we can see various information about each network device, such as its name, connection state, connection type, device type, and hardware address.

We can use other subcommands along with the `nmcli device` command to perform various actions on network devices, such as adding a new connection, modifying an existing connection, activating/deactivating a connection, and more. 

## tldr 
 
> Hardware device management with NetworkManager.
> This subcommand can also be called with `nmcli d`.
> More information: <https://networkmanager.dev/docs/api/latest/nmcli.html>.

- Print the statuses of all network interfaces:

`nmcli device status`

- Print the available Wi-Fi access points:

`nmcli device wifi`

- Connect to the Wi-Fi network with a specified name and password:

`nmcli device wifi connect {{ssid}} password {{password}}`

- Print password and QR code for the current Wi-Fi network:

`nmcli device wifi show-password`
