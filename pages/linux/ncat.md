# ncat 
## chatgpt 
ncat (or netcat) is a command-line utility used for reading from and writing to network connections using TCP or UDP protocols. It is commonly used for testing network connections, port scanning, and transferring data between systems.

The basic syntax for ncat command is:

ncat [options] [hostname] [port]

Here, [options] represent various options to customize the behavior of the command, [hostname] specifies the destination host to connect to, and [port] specifies the destination port to connect to.

Some of the commonly used options with ncat command are:

- -v: Enables verbose output that provides additional information about the connection.
- -u: Uses UDP protocol instead of the default TCP protocol.
- -l: Listens for incoming connections instead of making an outgoing connection.
- -p: Specifies the source port to use for outgoing connections.
- -e: Executes a command after establishing a connection.

For example, to connect to a remote host using TCP protocol on port 80, we can use the following command:

ncat example.com 80

This will initiate a TCP connection to example.com on port 80. Similarly, we can use the -l option to listen for incoming connections on a specific port:

ncat -l 8080

This will listen for incoming connections on port 8080. We can then use another ncat command from a remote machine to initiate an outgoing connection to this server:

ncat server_ip 8080

This will initiate a TCP connection to the server IP address on port 8080. 

## tldr 
 
> Use the normal `cat` functionality over networks.
> More information: <https://manned.org/ncat>.

- Listen for input on the specified port and write it to the specified file:

`ncat -l {{port}} > {{path/to/file}}`

- Accept multiple connections and keep ncat open after they have been closed:

`ncat -lk {{port}}`

- Write output of specified file to the specified host on the specified port:

`ncat {{address}} {{port}} < {{path/to/file}}`
