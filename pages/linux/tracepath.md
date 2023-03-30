# tracepath 
## chatgpt 
The `tracepath` command is a Linux utility used to trace the route path packets take from the source to the destination. It is similar to the `traceroute` command but has some additional functionalities such as the ability to trace the path for TCP, UDP or ICMP traffic, and allowing for more customization.

Syntax:
```
tracepath [options] hostname/IP_address/port
```

Options:
- `-n` — Display IP addresses instead of hostnames
- `-M` — Set maximum number of hops
- `-p` — Set the destination port number for UDP or TCP packets
- `-q` — Set the number of probes per hop
- `-w` — Set the timeout in seconds for each probe
- `-b` — Send broadcast packets
- `-g` — Use a gateway as the first hop

Example:
```
tracepath -n google.com
```
This command will trace the route path to `google.com` and display the list of IP addresses from source to destination.  

## tldr 
 
> Trace the path to a network host discovering MTU along this path.
> More information: <https://manned.org/tracepath>.

- A preferred way to trace the path to a host:

`tracepath -p {{33434}} {{host}}`

- Specify the initial destination port, useful with non-standard firewall settings:

`tracepath -p {{destination_port}} {{host}} `

- Print both hostnames and numerical IP addresses:

`tracepath -b {{host}}`

- Specify a maximum TTL (number of hops):

`tracepath -m {{max_hops}} {{host}}`

- Specify the initial packet length (defaults to 65535 for IPv4 and 128000 for IPv6):

`tracepath -l {{packet_length}} {{host}}`

- Use only IPv6 addresses:

`tracepath -6 {{host}}`
