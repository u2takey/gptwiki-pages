# tshark 
## chatgpt 
Tshark is a command-line network protocol analyzer tool that allows users to capture and analyze network traffic in real-time. The command "tshark" is used to launch the Tshark tool and start capturing and analyzing network traffic. When executed without any parameters, tshark displays a live list of all network traffic on the specified interface(s).

Some of the various command-line options that can be used with tshark include:

-c – Specifies the number of packets to capture before stopping.

-r – Allows tshark to read from a previously captured pcap file instead of directly capturing network traffic.

-w – Writes the output of tshark to a file instead of displaying it on the console.

-i – Specifies the network interface to capture traffic on.

-d – Allows users to specify additional protocol layers or protocols to decode.

-t – Specifies the format of the timestamps included in the output.

-T – Allows users to specify the format of the output.

-s – Specifies the size of the capture buffer.

-dns – Enables tshark to perform DNS name resolutions on captured packets.

Overall, tshark is a powerful tool that can be used to capture, filter, and analyze network traffic in real-time or from previously captured pcap files. Its extensive command-line options make it highly customizable and useful for debugging network issues, testing network functionality, and monitoring network security. 

## tldr 
 
> Packet analysis tool, CLI version of Wireshark.
> More information: <https://tshark.dev/>.

- Monitor everything on localhost:

`tshark`

- Only capture packets matching a specific capture filter:

`tshark -f '{{udp port 53}}'`

- Only show packets matching a specific output filter:

`tshark -Y '{{http.request.method == "GET"}}'`

- Decode a TCP port using a specific protocol (e.g. HTTP):

`tshark -d tcp.port=={{8888}},{{http}}`

- Specify the format of captured output:

`tshark -T {{json|text|ps|…}}`

- Select specific fields to output:

`tshark -T {{fields|ek|json|pdml}} -e {{http.request.method}} -e {{ip.src}}`

- Write captured packet to a file:

`tshark -w {{path/to/file}}`

- Analyze packets from a file:

`tshark -r {{path/to/file.pcap}}`
