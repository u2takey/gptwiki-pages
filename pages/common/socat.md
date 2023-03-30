# socat 
## chatgpt 
Socat is a command-line utility that allows users to create bidirectional streams between two endpoints, such as sockets or files, and can modify or analyze them in real-time.

The basic syntax of the socat command is as follows:

```
socat [options] <address 1> <address 2>
```

Here, `<address 1>` and `<address 2>` represent the two endpoints between which the stream is to be created. These endpoints can be of various types, such as:

- TCP/UDP sockets
- UNIX domain sockets
- PTYs (pseudo-terminals)
- Files

Socat also supports a wide range of options, which can be used to modify its behavior based on the specific requirements of the user. Some common options used with the socat command include:

- `-v` for verbose mode, which provides additional information during the transfer
- `-d` for debugging mode, which prints information about each step of the transfer
- `-x` for hexadecimal dump mode, which displays the transfer data in hexadecimal format

Example usage of the socat command:

To create a TCP socket and forward data from it to a file:

```
$ socat TCP-LISTEN:8080,reuseaddr,fork OPEN:/var/log/mylog.txt,creat,append
```

Here, we are listening for incoming TCP connections on port 8080 (`TCP-LISTEN:8080`) and forwarding incoming data to a file (`OPEN:/var/log/mylog.txt`). The `reuseaddr` and `fork` options are used to allow multiple clients to connect to the server simultaneously, while the `creat` and `append` options ensure that the file is created if it does not exist, and that data is appended to it instead of overwriting it. 

## tldr 
 
> Multipurpose relay (SOcket CAT).
> More information: <http://www.dest-unreach.org/socat/>.

- Listen to a port, wait for an incoming connection and transfer data to STDIO:

`socat - TCP-LISTEN:8080,fork`

- Create a connection to a host and port, transfer data in STDIO to connected host:

`socat - TCP4:www.example.com:80`

- Forward incoming data of a local port to another host and port:

`socat TCP-LISTEN:80,fork TCP4:www.example.com:80`
