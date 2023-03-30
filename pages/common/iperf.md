# iperf 
## chatgpt 
iperf is a command-line tool that is used to measure the network performance by initiating a TCP/UDP data stream between two network devices. It is commonly used for network bandwidth testing and troubleshooting.

Here's a brief overview of how to use the iperf command:

1. Install iperf: If iperf is not already installed on your computer, you need to install it first. Depending on your operating system, you can use the package manager or download the binary from the official website.

2. Choose the mode: Before running the iperf command, you need to decide which mode you want to use. There are two modes of iperf: client and server.

3. Start the server: If you're running the server mode, start the server by running the iperf command with the -s (or --server) option.

4. Start the client: If you're running the client mode, start the client by running the iperf command with the server's IP address or hostname.

5. Configure additional options: There are additional options you can configure to customize the iperf command with various parameters. For example, you can specify the port number, the protocol (TCP or UDP), the rate at which data is sent, etc.

6. Display the results: After the iperf session is complete, you will get a report on the network performance that includes details on the amount of data transmitted, the transfer rate, and any errors encountered during the test.

Overall, the iperf command is a powerful tool for measuring network performance and diagnosing network problems. It is widely used by network administrators, software developers, and other IT professionals to optimize their networks and ensure they run smoothly. 

## tldr 
 
> Measure network bandwidth between computers.
> More information: <https://iperf.fr>.

- Run on server:

`iperf -s`

- Run on server using UDP mode and set server port to listen on 5001:

`iperf -u -s -p {{5001}}`

- Run on client:

`iperf -c {{server_address}}`

- Run on client every 2 seconds:

`iperf -c {{server_address}} -i {{2}}`

- Run on client with 5 parallel threads:

`iperf -c {{server_address}} -P {{5}}`

- Run on client using UDP mode:

`iperf -u -c {{server_address}} -p {{5001}}`
