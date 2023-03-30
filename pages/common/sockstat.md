# sockstat 
## chatgpt 
The sockstat command is a UNIX command that displays information about open sockets on a system. It is typically used to view information about network connections that are currently active or being used by a program.

When the command is run, it displays a list of all open sockets, including their respective protocol, local and foreign address, and the state of the socket. The socket states can be one of the following:

- ESTABLISHED: The socket has an established connection.
- CLOSE_WAIT: The remote end has closed the connection, but the local end has not yet closed the connection.
- TIME_WAIT: The socket is waiting to ensure that all packets from the remote end have been received before closing the connection.
- CLOSED: The socket has been closed and is no longer in use.

The sockstat command is useful for troubleshooting networking issues and identifying the processes that are using certain ports or IP addresses. It can be run with various options to filter or sort the output, such as filtering by a specific protocol, user or process ID, or sorting by address or connection state. 

## tldr 
 
> List open Internet or UNIX domain sockets.
> More information: <https://www.freebsd.org/cgi/man.cgi?query=sockstat&sektion=1>.

- View which users/processes are listening to which ports:

`sockstat -l`
