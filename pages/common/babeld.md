# babeld 
## chatgpt 
Babeld is a routing daemon that implements the Babel protocol. It is used to exchange routing information in computer networks. Here is the detail of the babeld command:

Syntax:
```
babeld [OPTIONS] [INTERFACE ...]
```

The babeld command takes several options and one or more interfaces as arguments. The options include:

- `-d`: Enable debug mode. This option produces more verbose output that can be useful for troubleshooting.
- `-D`: Enable daemon mode. This option causes babeld to run in the background as a system service.
- `-c`: Specify a configuration file. This option allows you to specify a configuration file that contains additional settings and options for babeld.
- `-p`: Specify the port number. This option sets the port number that babeld will use to listen for incoming Babel packets.
- `-s`: Specify the source address. This option specifies the IP address that babeld will use as the source address when sending Babel packets.
- `-v`: Display version information. This option displays the version number and build information for babeld.

After the options, you can specify one or more network interfaces that babeld should use for sending and receiving Babel packets. These interfaces can be physical network interfaces (such as eth0) or virtual interfaces (such as tun0).

When you start babeld, it will begin listening for Babel packets on the specified interfaces and will initiate the exchange of routing information with other nodes on the network. It will also update its own routing table based on the information it receives from other nodes. 

## tldr 
 
> Routing daemon for Babel which uses firewall-style filters.
> More information: <https://www.irif.fr/~jch/software/babel/babeld.html>.

- Start babeld with a specific configuration file:

`babeld -c {{path/to/babeld.conf}}`

- Start babeld with multiple configuration files (read in order):

`babeld -c {{path/to/ports.conf}} -c {{path/to/filters.conf}} -c {{path/to/interfaces.conf}}`

- Start babeld and daemonise afterwards:

`babeld -D`

- Start babeld and pass a configuration command:

`babeld -C {{'redistribute metric 256'}}`

- Start babeld and specify on which interfaces to operate:

`babeld {{eth0}} {{eth1}} {{wlan0}}`
