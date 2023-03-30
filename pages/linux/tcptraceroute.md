# tcptraceroute 
## chatgpt 
tcptraceroute is a command-line tool that is used to trace the route taken by TCP packets from a source to a destination host. It works similar to traceroute command but sends TCP packets instead of ICMP packets to diagnose network connections.

The syntax of the tcptraceroute command is as follows:

```
tcptraceroute [options] host [port]
```

Here, 

- `host` : The IP address or hostname of the destination server that you want to trace.
- `port` : The port number on which you want to send TCP packets. This parameter is optional.

Some of the commonly used options with the tcptraceroute command are:

- `-f` : This option is used to specify the initial TTL (Time To Live) value of the TCP packets that are sent.
- `-m` : This option is used to set the maximum number of hops that tcptraceroute should trace before giving up. 
- `-n` : This option disables name lookup for each hop to speed up the output.
- `-w` : This option sets the timeout value for each probe in milliseconds.
- `-S` : This option allows you to set the source IP address of the packets that are sent.

When you run the tcptraceroute command with the specified options and arguments, it sends a series of TCP packets with increasing TTL values. With each TTL, the packet travels further through the network until it reaches the destination host. Along the way, each router or network device that handles the packet decreases the TTL value until the packet is either delivered or discarded due to a expired TTL. In case of successful delivery, the tcptraceroute command records the IP address, hostname and round-trip delay of each intermediate router that is traversed. This information is then used to build a map of the network path taken by the packets, thereby revealing problem areas such as network congestion or packet drops. 

## tldr 
 
> A traceroute implementation using TCP packets.
> More information: <https://github.com/mct/tcptraceroute>.

- Trace the route to a host:

`tcptraceroute {{host}}`

- Specify the destination port and packet length in bytes:

`tcptraceroute {{host}} {{destination_port}} {{packet_length}}`

- Specify the local source port and source address:

`tcptraceroute {{host}} -p {{source_port}} -s {{source_address}}`

- Set the first and maximum TTL:

`tcptraceroute {{host}} -f {{first_ttl}} -m {{max_ttl}}`

- Specify the wait time and number of queries per hop:

`tcptraceroute {{host}} -w {{wait_time}} -q {{number_of_queries}}`

- Specify the interface:

`tcptraceroute {{host}} -i {{interface}}`
