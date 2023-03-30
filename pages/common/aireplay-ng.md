# aireplay-ng 
## chatgpt 
aireplay-ng is a powerful command-line tool used for wireless network packet injection, testing, and other network-related tasks. This tool is often used alongside other tools in the Aircrack-ng suite for wireless network security testing.

The 'aireplay-ng' command can be used to launch a variety of attacks on wireless networks, including deauthentication attacks, fake access point (AP) creation, packet injection attacks, and more.

Some of the main options and parameters supported by the 'aireplay-ng' command include:

- '-0' or '--deauth': This option can be used to launch deauthentication attacks against clients on a wireless network. This can be used to force clients to reconnect and reveal their encryption keys, or to disrupt traffic on the network.

- '-1' or '--fakeauth': This option can be used to perform fake authentication to an access point, allowing the attacker to capture data packets from the network.

- '-3' or '--arpreplay': This option performs ARP request replay attacks that generate new ARP requests to potentially capture packets, and to disrupt a network.

- '-6' or '--inject': This option is used to inject packets into a wireless network, which can be used to generate traffic or carry out other attacks.

- '-9' or '--test': This option is used to test wireless networks for vulnerabilities, or to check the reliability of the wireless network.

Other options include setting the injection rate or specifying a specific network interface.

Overall, the 'aireplay-ng' command is a highly useful tool for anyone performing wireless network security testing or penetration testing, but it should be used with caution and its effectiveness is subject to many factors. 

## tldr 
 
> Inject packets into a wireless network.
> Part of `aircrack-ng`.
> More information: <https://www.aircrack-ng.org/doku.php?id=aireplay-ng>.

- Send a specific number of disassociate packets given an access point's MAC address, a client's MAC address and an interface:

`sudo aireplay-ng --deauth {{count}} --bssid {{ap_mac}} --dmac {{client_mac}} {{interface}}`
