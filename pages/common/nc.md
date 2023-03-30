# nc 
## chatgpt 
The nc command, also known as netcat, is a network utility tool used for reading and writing to network connections. It can be used for testing connections, port scanning, and transferring data over the network. Here are the details of the various flags that can be used with the nc command:

- `-l`: This flag tells nc to listen for incoming connections. It is used to set up a server that can accept incoming connections. This is often used with the `-p` flag to specify the port number on which to listen.

- `-p`: This flag is used to specify the port number on which to listen or the port number to which to connect. It is used along with the `-l` flag to set up a server that can accept incoming connections.

- `-u`: This flag is used to specify that nc should use UDP instead of TCP for the connection.

- `-v`: This flag is used to enable verbose mode, which displays more information about the network connection activity.

- `-n`: This flag is used to disable DNS lookup, which can speed up connection establishment in some cases.

- `-z`: This flag is used to specify that nc should scan for open ports and report back whether a connection can be established. This is often used as a quick way to test network connectivity.

- `-e`: This flag is used to specify a program to be executed after a connection is established. This is sometimes used for remote shell access.

- `-i`: This flag is used to specify the wait time in seconds between each connection attempt in a scan.

Overall, the nc command is a powerful tool for network connections and provides a lot of flexibility for configuring and testing network communications. 

## tldr 
 
> Netcat is a versatile utility for working with TCP or UDP data.
> More information: <https://nmap.org/ncat>.

- Listen on a specified port and print any data received:

`nc -l {{port}}`

- Connect to a certain port:

`nc {{ip_address}} {{port}}`

- Set a timeout:

`nc -w {{timeout_in_seconds}} {{ipaddress}} {{port}}`

- Keep the server up after the client detaches:

`nc -k -l {{port}}`

- Keep the client up even after EOF:

`nc -q {{timeout}} {{ip_address}}`

- Scan the open ports of a specified host:

`nc -v -z {{ip_address}} {{port}}`

- Act as proxy and forward data from a local TCP port to the given remote host:

`nc -l {{local_port}} | nc {{hostname}} {{remote_port}}`
