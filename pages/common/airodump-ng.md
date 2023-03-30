# airodump-ng 
## chatgpt 
The command "airodump-ng" is a tool used to capture wireless network traffic, including data frames and management frames. It is commonly used in wireless network testing and troubleshooting.

Here is a breakdown of the command:

- "airdump-ng" is the name of the command. It is preceded by "airodump-" because it is a part of the Aircrack-ng suite, which is a collection of wireless network security tools.

- The "-ng" part of the command stands for "next generation" and refers to the fact that this version of the tool is an update of the original Airodump tool.

- The command is typically used in the terminal or command prompt on a computer running Linux or other Unix-based operating system.

- The tool scans for wireless networks in range and displays information about each network, including the SSID (network name), MAC address of the access point, channel, and security information.

- The tool can also be used to capture and analyze packets on a particular wireless network for more detailed troubleshooting or security testing.

Overall, the "airodump-ng" command is a powerful tool for anyone working with wireless networks, allowing them to easily capture and analyze network traffic. 

## tldr 
 
> Capture packets and display information about wireless networks.
> Part of `aircrack-ng`.
> More information: <https://www.aircrack-ng.org/doku.php?id=airodump-ng>.

- Capture packets and display information about a wireless network:

`sudo airodump-ng {{interface}}`

- Capture packets and display information about a wireless network given the MAC address and channel, and save the output to a file:

`sudo airodump-ng --channel {{channel}} --write {{path/to/file}} --bssid {{mac}} {{interface}}`
