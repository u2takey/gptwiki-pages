# macchanger 
## chatgpt 
The 'macchanger' command is a Linux utility that is used to change the Media Access Control (MAC) address of a network interface. The MAC address is a unique identifier assigned to a network interface, and it is used to identify the device on the network.

The 'macchanger' command can be used to change the MAC address of both wireless and wired network interfaces. It can be useful in situations where you want to hide your device from the network, bypass MAC address filtering, or just generally increase the privacy and security of your network connection.

The general syntax for using the 'macchanger' command is as follows:

$ macchanger [options] interface

Where 'interface' is the name of the network interface whose MAC address you want to change.

Some frequently used options with macchanger command are:

- -r, --random: This option sets a random MAC address for the interface.
- -p, --permanent: This option sets a permanent MAC address for the interface.
- -a, --another: This option sets the MAC address of another device on the network.
- -s, --show: This option displays the current MAC address of the interface.

For example, if you want to change the MAC address of your wireless interface named 'wlan0' to a randomly generated MAC address, you can use the following command:

$ sudo macchanger -r wlan0

The above command will create a random MAC address for the 'wlan0' interface, which can then be used to connect to the network.

It is important to note that changing the MAC address may be illegal in certain countries or situations, and it can also cause compatibility issues with certain network devices or services. Therefore, it is recommended to use this command with caution and only for legitimate purposes. 

## tldr 
 
> Command-line utility for manipulating network interface MAC addresses.
> More information: <https://manned.org/macchanger>.

- View the current and permanent MAC addresses of a interface:

`macchanger --show {{interface}}`

- Set interface to a random MAC:

`macchanger --random {{interface}}`

- Set interface to a specific MAC:

`macchanger --mac {{XX:XX:XX:XX:XX:XX}} {{interface}}`

- Reset interface to its permanent hardware MAC:

`macchanger --permanent {{interface}}`
