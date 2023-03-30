# wpa_supplicant 
## chatgpt 
wpa_supplicant is a command-line utility used for configuring and managing wireless network connections in Linux operating systems. It is used as a client-side Wi-Fi software that implements the WPA and WPA2 security protocols on wireless networks.

When executed, the wpa_supplicant command can be used to configure and manage various network settings using different command-line options. These options include:

- -i: Specifies the network interface to be used for the wireless connection.
- -c: Specifies the path to the configuration file that contains the network settings.
- -D: Specifies the wireless driver to be used.
- -B: Runs wpa_supplicant in the background.
- -dd: Enables verbose debugging output.

The key feature of wpa_supplicant is its ability to securely authenticate to wireless networks using protocols such as WPA and WPA2. It can also be used to connect to open and hidden SSIDs, perform automatic network selection and roaming, and manage multiple simultaneous connections.

Overall, wpa_supplicant is a powerful and customizable tool that helps Linux users to establish secure Wi-Fi connections with ease. 

## tldr 
 
> Manage protected wireless networks.
> More information: <https://manned.org/wpa_supplicant.1>.

- Join a protected wireless network:

`wpa_supplicant -i {{interface}} -c {{path/to/wpa_supplicant_conf.conf}}`

- Join a protected wireless network and run it in a daemon:

`wpa_supplicant -B -i {{interface}} -c {{path/to/wpa_supplicant_conf.conf}}`
