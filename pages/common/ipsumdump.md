# ipsumdump 
## chatgpt 
Ipsumdump is a command-line tool in Linux that extracts content from an IP packet capture file in a human-readable format. It displays the contents of the packet capture file in the format of the packet header and the payload (the data contained in the packet).

The command structure for ipsumdump is as follows:

`ipsumdump [options] <filename>`

Where:

- `ipsumdump` is the command name.
- `[options]` are additional command line options that can be used to customize the output format or filter the content of the capture file.
- `<filename>` is the path to the capture file that is going to be analyzed.

Some of the most commonly used options for ipsumdump are:

- `-r`: Reads packets from a specified capture file.
- `-c`: Limits the number of packets to display.
- `-e`: Displays extended information about each packet.
- `-l`: Specifies the number of hexadecimal data bytes displayed per line.
- `-n`: Displays the packet payload in ASCII characters instead of hexadecimal data.

For example, the following command will read the contents of "capture.pcap" and display the first 10 packets in ASCII format:

`ipsumdump -r capture.pcap -c 10 -n`

The output will include information about each packet, such as the source and destination IP addresses, protocol, and payload. The payload will be displayed in ASCII format instead of hexadecimal data.

In summary, ipsumdump is a tool that helps network administrators and security experts to analyze and interpret packet capture files. Its ability to display the captured packets in a human-readable format is crucial for understanding the behavior of the network and identifying potential security issues. 

## tldr 
 
> Summarise TCP/IP dumps into a human and machine readable ASCII format.
> More information: <https://manned.org/ipsumdump>.

- Print the source and destination IP addresses of all packets in a pcap file:

`ipsumdump --src --dst {{path/to/file.pcap}}`

- Print the timestamps, source address, source port, destination address, destination port and protocol of all packets read from a given network interface:

`ipsumdump --interface {{eth0}} -tsSdDp`

- Print the anonymised source address, anonymised destination address, and IP packet length of all packets in a pcap file:

`ipsumdump --src --dst --length --anonymize {{path/to/file.pcap}}`
