# traceroute 
## chatgpt 
Traceroute is a command-line tool for network analysis which is used to track the path of packets through an Internet Protocol (IP) network. By sending packets with gradually increasing Time To Live (TTL) values through the network and measuring the time it takes for the packets to reach the destination, traceroute can determine the route the packets are taking and identify any possible problems along the way.

Here is the syntax of the traceroute command:

```
traceroute [-FIldnrv] [-f first_ttl] [-m max_ttl] [-p port] [-q nqueries] [-s src_addr] [-t tos] [-w wait_time] host [packet_length]
```

Here are the main options and what they do:

- `-F`: This option specifies the use of the IP "Don't Fragment" flag.
- `-I`: This option uses ICMP Echo Request packets instead of UDP datagrams.
- `-l`: This option uses a loose source route.
- `-d`: This option sets the "TCP-style" output format, which shows the complete TCP connection state for each attempt.
- `-n`: This option disables hostname lookup and displays IP addresses instead.
- `-r`: This option disables the reverse hostname lookup.
- `-v`: This option enables verbose output.
- `-f first_ttl`: This option sets the initial Time To Live (TTL) value.
- `-m max_ttl`: This option sets the maximum TTL value.
- `-p port`: This option sets the UDP port number to be used.
- `-q nqueries`: This option sets the number of probes per TTL value.
- `-s src_addr`: This option sets the source IP address.
- `-t tos`: This option sets the Type of Service (TOS) value.
- `-w wait_time`: This option sets the number of seconds to wait for a response.

The syntax of the traceroute command is fairly complex, so it's important to be familiar with what each option does in order to use it effectively. 

## tldr 
 
> Print the route packets trace to network host.
> More information: <https://manned.org/traceroute>.

- Traceroute to a host:

`traceroute {{host}}`

- Disable IP address and host name mapping:

`traceroute -n {{host}}`

- Specify wait time for response:

`traceroute -w {{0.5}} {{host}}`

- Specify number of queries per hop:

`traceroute -q {{5}} {{host}}`

- Specify size in bytes of probing packet:

`traceroute {{host}} {{42}}`
