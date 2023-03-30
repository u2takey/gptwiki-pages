# iw 
## chatgpt 
The "iw" command is used on Linux systems to configure and manage wireless network interfaces. It is a command-line tool that works with the nl80211 kernel interface to communicate with the wireless driver.

Some of the common uses of the "iw" command include:

1. Displaying Wireless Network Information: The "iw" command can be used to display detailed information about the wireless network interface on your system, including the current configuration, supported frequencies, channel utilization, signal strength, and more.

2. Scanning for Wireless Networks: The "iw" command can be used to initiate a scan for available wireless networks in the vicinity.

3. Configuring Wireless Network Settings: The "iw" command can also be used to configure various wireless network settings, such as setting the channel, frequency, modulation, and encryption parameters.

4. Monitoring Wireless Network Traffic: The "iw" command can be used with other tools, such as tcpdump, to monitor wireless network traffic and analyze network behavior.

Overall, the "iw" command is a powerful tool for working with wireless networks on Linux systems. It provides a range of functionality for managing and analyzing wireless network settings, and can be used in a variety of different applications. 

## tldr 
 
> Show and manipulate wireless devices.
> More information: <https://manned.org/iw>.

- Scan for available wireless networks:

`iw dev {{wlp}} scan`

- Join an open wireless network:

`iw dev {{wlp}} connect {{SSID}}`

- Close the current connection:

`iw dev {{wlp}} disconnect`

- Show information about the current connection:

`iw dev {{wlp}} link`
