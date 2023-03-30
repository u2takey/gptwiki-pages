# tcpflow 
## chatgpt 
Tcpflow is a command-line tool that captures data transmitted as TCP connections between two computers or devices, and it separates each stream into its own file, making it easier to analyze and inspect the contents of the data. 

Here are some of the most commonly used options with tcpflow:

1. -i [interface]: lets you specify the network interface to listen on. For example, "tcpflow -i eth0" will capture traffic on the "eth0" network interface.

2. -p [port]: filters traffic based on the specified TCP port number. For example, "tcpflow -p 80" captures traffic on port 80 (HTTP).

3. -c: captures both sides of the TCP connection. By default, tcpflow only captures traffic coming to the local machine.

4. -r [file]: reads a previously captured pcap file instead of listening live on a network interface.

5. -w [file]: writes the output to a specified file instead of printing it to the command line.

To use tcpflow, simply run the command followed by any options or filters you want to apply. If tcpflow is listening on a network interface, it will capture all TCP traffic that matches the filters you specified, and it will create separate output files for each TCP stream. The output files will be located in the current working directory unless you specify a different location with the "-w" option. 

Tcpflow can be used for a variety of purposes, such as troubleshooting network issues, analyzing network protocols, and extracting data from network transmissions. It is a powerful and versatile tool that comes in handy when you need to inspect the contents of network traffic. 

## tldr 
 
> Capture TCP traffic for debugging and analysis.
> More information: <https://manned.org/tcpflow>.

- Show all data on the given interface and port:

`tcpflow -c -i {{eth0}} port {{80}}`
