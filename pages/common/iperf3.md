# iperf3 
## chatgpt 
iperf3 is a command-line tool that can be used to measure network performance by generating and sending data between two devices. The tool supports a variety of parameters that allow for customization of the testing environment and can provide highly detailed information on network performance.

The iperf3 command begins with the name of the program, followed by various arguments to configure the test. Some of the more common options that can be used include:

- -s: Configures the program to operate as a server, listening for incoming connections from clients.
- -c <ip address>: Configures the program to operate as a client and connect to a server at the specified IP address.
- -u: Configures the program to use UDP instead of TCP, which can be useful for testing real-time applications like voice or video over IP.
- -p <port>: Specifies the port number that the server should listen on or the client should connect to.
- -M <packet size>: Sets the maximum size of data packets that should be sent during the test.
- -i <interval>: Specifies the interval at which results should be displayed.

Once the command is executed, iperf3 will begin sending data between the two devices and measuring the performance of the network. The results of the test will be displayed on the terminal screen, including information on data transfer rates, packet loss, and jitter. This information can be used to identify potential problems on the network and make adjustments to improve network performance. 

## tldr 
 
> Traffic generator for testing network bandwidth.
> More information: <https://iperf.fr>.

- Run iperf3 as a server:

`iperf3 -s`

- Run an iperf3 server on a specific port:

`iperf3 -s -p {{port}}`

- Start bandwidth test:

`iperf3 -c {{server}}`

- Run iperf3 in multiple parallel streams:

`iperf3 -c {{server}} -P {{streams}}`

- Reverse direction of the test. Server sends data to the client:

`iperf3 -c {{server}} -R`
