# dumpcap 
## chatgpt 
Dumpcap is a command-line network packet capture tool that is included in Wireshark, the popular network protocol analyzer. When run, dumpcap captures network traffic from an interface on the system and either saves it to a file or displays it to the console.

Here are some common options used with the dumpcap command:

- `-i <interface>` specifies the network interface to capture traffic from. For example, `-i eth0` would capture traffic on the first Ethernet interface.
- `-w <filename>` specifies the file name to save the captured packets to. For example, `-w capture.pcap` would save the packets to a file called "capture.pcap".
- `-c <count>` specifies the number of packets to capture before stopping. For example, `-c 100` would capture 100 packets and then stop.
- `-f <filter>` specifies a capture filter to use when capturing packets. For example, `-f "host 192.168.1.1"` would capture packets only to/from the IP address 192.168.1.1.

Overall, dumpcap is a powerful and versatile tool for capturing and analyzing network traffic. It allows you to collect detailed information about network activity, diagnose network issues, and troubleshoot problems with network applications. 

## tldr 
 
> A network traffic dump tool.
> More information: <https://www.wireshark.org/docs/man-pages/dumpcap.html>.

- Display available interfaces:

`dumpcap --list-interfaces`

- Capture packets on a specific interface:

`dumpcap --interface {{1}}`

- Capture packets to a specific location:

`dumpcap --interface {{1}} -w {{path/to/output_file.pcapng}}`

- Write to a ring buffer with a specific max file limit of a specific size:

`dumpcap --interface {{1}} -w {{path/to/output_file.pcapng}} --ring-buffer filesize:{{500000}} --ring-buffer files:{{10}}`
