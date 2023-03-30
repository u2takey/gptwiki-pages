# iftop 
## chatgpt 
The `iftop` command is an interactive command-line utility that displays real-time network interface bandwidth usage for a network interface. It shows the traffic rates for incoming and outgoing traffic for each network connection or host, and can be used to monitor network traffic in real-time.

When you run the `iftop` command, you get an interface similar to the top command in Linux. It displays live traffic that is flowing through the network interface, including the source and destination IP addresses, the protocol type, and the data rate in real-time. 

The interface is divided into two sections: the top section shows a list of connections with their IP address and data transfer rates, while the bottom section displays a graph of the changing network utilization, updated every few seconds by default. 

There are several options available with the `iftop` command, such as selecting a network interface to monitor, specifying a filter to show only a certain type of traffic, setting a limit on the amount of data to be displayed, and more. 

Overall, the `iftop` command is a useful tool for network administrators or anyone who wants to monitor their network traffic in real-time, as it provides a clear and detailed picture of the traffic flowing through the network interface. 

## tldr 
 
> Show bandwidth usage on an interface by host.
> More information: <https://manned.org/iftop>.

- Show the bandwidth usage:

`sudo iftop`

- Show the bandwidth usage of a given interface:

`sudo iftop -i {{interface}}`

- Show the bandwidth usage with port information:

`sudo iftop -P`

- Do not show bar graphs of traffic:

`sudo iftop -b`

- Do not look up hostnames:

`sudo iftop -n`

- Get help about interactive commands:

`?`
