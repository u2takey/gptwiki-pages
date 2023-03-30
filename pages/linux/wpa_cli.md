# wpa_cli 
## chatgpt 
wpa_cli is a command-line interface for configuring and controlling the WPA Supplicant program, which is used to manage Wi-Fi networks on Linux systems. It allows you to interact with wpa_supplicant, which is responsible for managing Wi-Fi connections, such as connecting to a network, scanning for available networks, and configuring network security settings.

Some common uses of wpa_cli include:

- Connecting to a Wi-Fi network: wpa_cli can be used to scan for and connect to Wi-Fi networks. For example, the command "wpa_cli scan" will scan for available networks, and "wpa_cli add_network" will create a new network profile. You can then configure the profile with the appropriate SSID and security settings using the "wpa_cli set_network" command, and finally connect to the network with "wpa_cli enable_network".
- Monitoring Wi-Fi connection status: wpa_cli provides detailed information about the current Wi-Fi connection, such as signal strength, channel, and speed. You can use the "wpa_cli status" command to display this information.
- Setting Wi-Fi network parameters: wpa_cli can be used to set various Wi-Fi network parameters, such as the maximum transmission unit (MTU) size and the time interval for scanning for available networks. You can use the "wpa_cli set" command to set these and other parameters.

In short, wpa_cli is a powerful tool that allows you to configure and control Wi-Fi connections on Linux systems. 

## tldr 
 
> Add and configure wlan interfaces.
> More information: <https://manned.org/wpa_cli>.

- Scan for available networks:

`wpa_cli scan`

- Show scan results:

`wpa_cli scan_results`

- Add a network:

`wpa_cli add_network {{number}}`

- Set a network's SSID:

`wpa_cli set_network {{number}} ssid "{{SSID}}"`

- Enable network:

`wpa_cli enable_network {{number}}`

- Save config:

`wpa_cli save_config`
