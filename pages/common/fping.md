# fping 
## chatgpt 
`fping` is a network diagnostic tool used for pinging multiple hosts on a network simultaneously. Unlike the traditional `ping` command, which only pings one host at a time, `fping` can take a list of hosts as input and send ICMP packets to each one of them in parallel, thus giving a quick overview of the network status.

Here is the basic syntax of the `fping` command:

```
fping [options] host1 host2 host3 ...
```

Some of the most commonly used options of the `fping` command are:

- `-c`: Specifies the number of times to ping each host (default is 1).
- `-q`: Quiet mode, only shows the summary stats (no output for hosts that are alive).
- `-a`: Only shows the hosts that are alive (default is to show alive and dead hosts).
- `-g`: Generates a list of IP addresses based on a network address and subnet mask.
- `-r`: Randomizes the order of the hosts in the list to avoid any patterns or biases.

Example Usage:

1. To ping a single host:
```
fping google.com
```

2. To ping multiple hosts:
```
fping google.com yahoo.com reddit.com
```

3. To specify the number of times to ping each host:
```
fping -c 3 google.com yahoo.com reddit.com
```

4. To display only the list of alive hosts:
```
fping -a google.com yahoo.com reddit.com
```

5. To generate a list of IP addresses:
```
fping -g 192.168.1.0/24
```

Overall, `fping` is a versatile tool that can help you troubleshoot network issues and monitor the status of hosts on a network. 

## tldr 
 
> A more powerful ping which can ping multiple hosts.
> More information: <https://fping.org>.

- List alive hosts within a subnet generated from a netmask:

`fping -a -g 192.168.1.0/24`

- List alive hosts within a subnet generated from an IP range:

`fping -a -g 192.168.1.1 192.168.1.254`

- List unreachable hosts within a subnet generated from a netmask:

`fping -u -g 192.168.1.0/24`
