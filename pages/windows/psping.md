# psping 
## chatgpt 
Psping is a command-line tool used for network diagnostics and performance measurement. It’s a Windows-based tool that allows measuring TCP/UDP latency and bandwidth at the same time. It also tests network connectivity with other hosts.

Here's how to use the psping command:

1. To measure the latency (in milliseconds) between your workstation and a specific endpoint, execute the following command:

   psping <IP address or hostname>

   For example:
   
   psping 10.1.1.1

   This will test the latency between your workstation and the device with IP address 10.1.1.1.

2. To test the TCP port connectivity to a specific endpoint, run the following command:

   psping -t <IP address or hostname>:<Port>

   For example:
   
   psping -t 10.1.1.1:80

   This will test the TCP connectivity to the device with IP address 10.1.1.1 on port 80.

3. To test UDP connectivity to a specific endpoint, run the following command:

   psping -u <IP address or hostname>:<Port>

   For example:
   
   psping -u 10.1.1.1:53

   This will test the UDP connectivity to the device with IP address 10.1.1.1 on port 53.

4. To test the bandwidth (in megabits per second) between your workstation and a specific endpoint, run the following command:

   psping -b <IP address or hostname>

   For example:
   
   psping -b 10.1.1.1

   This will test the bandwidth between your workstation and the device with IP address 10.1.1.1.

The psping command is a helpful tool for network administrators or anyone who wants to troubleshoot network issues or test network performance. 

## tldr 
 
> A ping tool that includes TCP ping, latency and bandwidth measurement.
> More information: <https://learn.microsoft.com/sysinternals/downloads/psping>.

- Ping a host using ICMP:

`psping {{hostname}}`

- Ping a host over a TCP port:

`psping {{hostname}}:{{port}}`

- Specify the number of pings and perform it quietly:

`psping {{hostname}} -n {{pings}} -q`

- Ping the target over TCP 50 times and produce a histogram of the results:

`psping {{hostname}}:{{port}} -q -n {{50}} -h`

- Display usage information:

`psping /?`
