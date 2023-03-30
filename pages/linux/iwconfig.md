# iwconfig 
## chatgpt 
The "iwconfig" command is a Linux network utility command that allows users to configure and manage wireless network interfaces. This command is used to display the configuration of the wireless network interface, as well as to modify configurations such as wireless modes, SSID, encryption keys, and more.

Here are some of the key parameters used with the "iwconfig" command:

- interface name: the name of the wireless network interface, such as "wlan0"
- mode: specifies which wireless mode to use, such as "managed", "ad-hoc", or "monitor"
- frequency/channel: the frequency or channel on which to communicate with the wireless network
- ESSID: the SSID (Service Set Identifier) of the wireless network
- access point: the MAC address of the access point of the wireless network
- encryption type and key: the type of encryption used, such as WEP or WPA, and the encryption key used
- power management: allows users to turn power management on or off for the wireless adapter

Overall, the "iwconfig" command is a useful tool for managing wireless network interfaces on Linux systems, and allows users to easily configure and troubleshoot wireless network connections. 

## tldr 
 
> Configure and show the parameters of a wireless network interface.
> More information: <https://manned.org/iwconfig>.

- Show the parameters and statistics of all the interfaces:

`iwconfig`

- Show the parameters and statistics of the specified interface:

`iwconfig {{interface}}`

- Set the ESSID (network name) of the specified interface (e.g. eth0 or wlp2s0):

`iwconfig {{interface}} {{new_network_name}}`

- Set the operating mode of the specified interface:

`iwconfig {{interface}} mode {{ad hoc|Managed|Master|Repeater|Secondary|Monitor|Auto}}`
