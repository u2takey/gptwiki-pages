# pathping 
## chatgpt 
Pathping is a Windows-based command that provides information about network latency and packet loss on a particular route between the source and the destination. The command is used to detect network problems and causes of poor network performance. 

When the pathping command is executed, it sends out packets to each router in the route between the source and destination. Each router then sends back an ICMP message containing information about the latency and packet loss on its particular link. This information is then compiled by the command and displayed in a more detailed report than the traditional ping command.

The output of the pathping command shows detailed information about each router in the route, including hop count, round-trip time, packet loss, and other statistics for each hop. It also shows average latency and packet loss for each router.

The pathping command is useful in troubleshooting network problems because it provides a more detailed view of the network path than a simple ping. It also allows network administrators to spot weak links in the network, which can be the cause of performance issues or network outages.

Syntax:
pathping [-g host-list] [-h maximum_hops] [-i address] [-n] [-p period] [-q num_queries] [-w timeout] [-4] [-6] target_name

-g host-list: This option specifies a gateway or intermediate destination to be used with the target. You can specify up to nine gateways or intermediate destinations in a comma-separated list.

-h maximum_hops: This option specifies the maximum number of hops to search for the target. The default value is 30.

-i address: This option specifies the source address to use when pinging the target.

-n: This turns off the host name resolution.

-p period: This option specifies the number of milliseconds to wait between sending each packet.

-q num_queries: This option specifies the number of queries per hop. The default value is 100.

-w timeout: This option specifies the number of milliseconds to wait for a response before timing out.

-4: This option forces the use of IPv4 addressing.

-6: This option forces the use of IPv6 addressing.

target_name: This is the name or IP address of the target. 

## tldr 
 
> A trace route tool combining features of `ping` and `tracert`.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/pathping>.

- Ping and trace the route to a host:

`pathping {{hostname}}`

- Do not perform reverse lookup of IP address to hostname:

`pathping {{hostname}} -n`

- Specify the maximum number of hops to search for the target (the default is 30):

`pathping {{hostname}} -h {{max_hops}}`

- Specify the milliseconds to wait between pings (the default is 240):

`pathping {{hostname}} -p {{time}}`

- Specify the number of queries per hop (the default is 100):

`pathping {{hostname}} -q {{queries}}`

- Force IPV4 usage:

`pathping {{hostname}} -4`

- Force IPV6 usage:

`pathping {{hostname}} -6`

- Display detailed usage information:

`pathping /?`
