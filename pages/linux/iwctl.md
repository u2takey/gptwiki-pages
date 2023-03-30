# iwctl 
## chatgpt 
The "iwctl" command is used to manage and configure wireless network connections on a Linux system. It is a command-line interface that allows users to interact with the "iwd" daemon, which is a lightweight and secure daemon for managing wireless connections.

When the "iwctl" command is executed, it opens an interactive shell where users can input commands to manage wireless networks. Some common commands that can be used with "iwctl" include:

- "device list": this command lists all the wireless devices available on the system.
- "station [device name] scan": this command initiates a wireless network scan on the specified device to discover available wireless networks.
- "station [device name] connect [network name]": this command connects to the specified wireless network on the specified device.
- "station [device name] show": this command displays detailed information about the current wireless connection, such as the signal strength, IP address, and network speed.

Overall, "iwctl" provides a simple and efficient way to manage wireless networks on a Linux system without the need for a graphical user interface. 

## tldr 
 
> A command-line tool for controlling the iwd network supplicant.
> More information: <https://iwd.wiki.kernel.org/gettingstarted>.

- Start the interactive mode, in this mode you can enter the commands directly, with autocompletion:

`iwctl`

- Call general help:

`iwctl --help`

- Display your Wi-Fi stations:

`iwctl station list`

- Start looking for networks with a station:

`iwctl station {{station}} scan`

- Display the networks found by a station:

`iwctl station {{station}} get-networks`

- Connect to a network with a station, if credentials are needed they will be asked:

`iwctl station {{station}} connect {{network_name}}`
