# aircrack-ng 
## chatgpt 
Aircrack-ng is a command-line tool used for network analysis and password cracking. It is primarily used for cracking and breaking down WEP (Wired Equivalent Privacy) and WPA (Wi-Fi Protected Access) encryption. It is also used to test and monitor the security of Wi-Fi networks.

The commands in aircrack-ng are used to capture, crack and analyze wireless network packets. Here are some of the most common commands used in aircrack-ng:

- airodump-ng: This command is used to capture Wi-Fi network packets and save the data to a file. It allows you to identify nearby wireless networks, including their SSIDs, channels, and encryption types.

- aireplay-ng: This command is used to forge or replay wireless network packets to test the security of the network.

- aircrack-ng: This command is used to crack the encryption key of a vulnerable wireless network. It uses brute-force techniques to guess the password of the network.

- airmon-ng: This command is used to enable monitor mode on the wireless network interface. Monitor mode allows you to capture all wireless network traffic in the air, even that which is not intended for your computer.

Aircrack-ng is a powerful network analysis tool. However, it should be used only for ethical hacking purposes and with permission from the owner of the network being tested. Unauthorized access to a computer network is a criminal offense in many countries. 

## tldr 
 
> Crack WEP and WPA/WPA2 keys from handshake in captured packets.
> Part of Aircrack-ng network software suite.
> More information: <https://www.aircrack-ng.org/doku.php?id=aircrack-ng>.

- Crack key from capture file using [w]ordlist:

`aircrack-ng -w {{path/to/wordlist.txt}} {{path/to/capture.cap}}`

- Crack key from capture file using [w]ordlist and the access point's [e]ssid:

`aircrack-ng -w {{path/to/wordlist.txt}} -e {{essid}} {{path/to/capture.cap}}`

- Crack key from capture file using [w]ordlist and the access point's MAC address:

`aircrack-ng -w {{path/to/wordlist.txt}} --bssid {{mac}} {{path/to/capture.cap}}`
