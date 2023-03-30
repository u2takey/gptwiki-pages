# wol 
## chatgpt 
The "wol" command stands for "Wake-on-LAN" and is used to remotely wake up a computer or other device that supports Wake-on-LAN. Wake-on-LAN is a network protocol that allows a device to be awakened from a sleeping or powered-off state via a network message, typically sent using a network management tool or command line utility.

The syntax of the "wol" command typically includes the target device's MAC address, which is used to uniquely identify the device on the network, as well as optionally specifying a target broadcast address or network interface to be used for sending the wake-up message.

For example, to wake up a device with a MAC address of 00:11:22:33:44:55, you might use the following command:

wol 00:11:22:33:44:55

This would typically send a broadcast message to the local network, instructing any devices that recognize the target MAC address to wake up and resume normal operation.

Overall, the "wol" command can be a useful tool for remotely managing and waking up devices on a network, and is often used in enterprise or home automation scenarios where devices may need to be powered on or off at specific times or under specific conditions. 

## tldr 
 
> Client for sending Wake-on-LAN magic packets.
> More information: <https://sourceforge.net/projects/wake-on-lan/>.

- Send a WoL packet to a device:

`wol {{mac_address}}`

- Send a WoL packet to a device in another subnet based on its IP:

`wol --ipaddr={{ip_address}} {{mac_address}}`

- Send a WoL packet to a device in another subnet based on its hostname:

`wol --host={{hostname}} {{mac_address}}`

- Send a WoL packet to a specific port on a host:

`wol --port={{port_number}} {{mac_address}}`

- Read hardware addresses, IP addresses/hostnames, optional ports and SecureON passwords from a file:

`wol --file={{path/to/file}}`

- Turn on verbose output:

`wol --verbose {{mac_address}}`
