# arpspoof 
## chatgpt 
The arpspoof command is a network utility that allows an attacker to intercept and modify network packets between two devices on a Local Area Network (LAN). 

ARP spoofing is a technique in which an attacker broadcasts false ARP messages on a local network, tricking the devices on the network into believing that the attacker's device is the gateway or another device on the network. Once the attacker has successfully spoofed the ARP cache of the victim machine, they can intercept, modify, or redirect network traffic between the two machines.

The arpspoof command is a tool used for carrying out ARP spoofing attacks. It sends ARP packets to the target machine and the gateway, pretending to be the other device, in order to intercept and modify network traffic between them.

Here is the syntax of the arpspoof command:

arpspoof [-i interface] [-t target] [-r host] [options] [host]

Where:

- -i: Specify the network interface that the attacker is using to carry out the attack.
- -t: Specify the target device(s) that the attacker wants to intercept traffic from. This can be multiple targets separated by commas.
- -r: Specify the IP address of the device that is acting as the default gateway for the network.
- host: The hostname or IP address of the target device.

Some common options that can be used with arpspoof command include -v (verbose mode), -c (display ARP cache), -w (write packet capture file), and -s (set the source IP address).

It's important to note that ARP spoofing attacks can be detected and prevented by implementing certain security measures such as port security, VLANs, and ARP spoofing detection tools. It is also illegal to carry out ARP spoofing attacks on networks that the attacker does not have explicit authorization to access. 

## tldr 
 
> Forge ARP replies to intercept packets.
> More information: <https://monkey.org/~dugsong/dsniff>.

- Poison all hosts to intercept packets on [i]nterface for the host:

`sudo arpspoof -i {{wlan0}} {{host_ip}}`

- Poison [t]arget to intercept packets on [i]nterface for the host:

`sudo arpspoof -i {{wlan0}} -t {{target_ip}} {{host_ip}}`

- Poison both [t]arget and host to intercept packets on [i]nterface for the host:

`sudo arpspoof -i {{wlan0}} -r -t {{target_ip}} {{host_ip}}`
