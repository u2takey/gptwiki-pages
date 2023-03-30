# airmon-ng 
## chatgpt 
airmon-ng command is a tool used on Linux operating systems for monitoring and managing wireless network adapters that support monitor mode. It is used mainly for detecting and analyzing wireless networks and also helps in cracking the Wi-Fi credentials.

The airmon-ng command is made up of two parts, the "airmon" and the "ng." The "airmon" part of the command is used to put the wireless network adapter into monitor mode. The "ng" part of the command initiates the network card driver which helps detect wireless signals.

The command syntax is as follows:
airmon-ng [start|stop] [interface]

The parameter "start" tells airmon-ng to start monitor mode. The parameter "stop" tells airmon-ng to stop monitor mode. The parameter "interface" is the name of the wireless network adapter.

Example: To start monitor mode on wlan0 interface, we can use the following command:
airmon-ng start wlan0

Once monitor mode is started, we can use other tools like Wireshark to capture and analyze wireless network traffic. 

Note: It is important to note that using airmon-ng command for hacking Wi-Fi networks without proper authorization is illegal and unethical. 

## tldr 
 
> Activate monitor mode on wireless network devices.
> Part of `aircrack-ng`.
> More information: <https://www.aircrack-ng.org/doku.php?id=airmon-ng>.

- List wireless devices and their statuses:

`sudo airmon-ng`

- Turn on monitor mode for a specific device:

`sudo airmon-ng start {{wlan0}}`

- Kill disturbing processes that use wireless devices:

`sudo airmon-ng check kill`

- Turn off monitor mode for a specific network interface:

`sudo airmon-ng stop {{wlan0mon}}`
