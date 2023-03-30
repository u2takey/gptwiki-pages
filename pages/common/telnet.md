# telnet 
## chatgpt 
The "telnet" command is a terminal emulation protocol. It allows a user to connect to a remote host or server using the Telnet protocol, which is a network protocol used to provide a bidirectional interactive text-oriented communication facility over the Internet.

When you type the "telnet" command with a specific hostname or IP address as a parameter, it initiates an open in the Telnet protocol on port 23. This creates a virtual terminal session that allows you to interact with the remote host as if you were sitting in front of the computer. The telnet command opens a connection to the specified IP address or hostname on the specified port and can be used to exchange text data between the local machine and the remote host.

Once the connection is established, you can communicate with the remote host through the terminal window using various commands and protocols supported by Telnet. These commands can be used to control and manipulate the remote system, or to transfer data between the local and remote machines.

Overall, the telnet command is a powerful tool that allows users to remotely access and control other systems over the Internet, providing a crucial function for network administration, system maintenance, and troubleshooting. It is important to note, however, that Telnet is an unsecured protocol and may transmit sensitive information in cleartext, so it is not recommended for use over the public Internet without additional encryption or security protocols in place. 

## tldr 
 
> Connect to a specified port of a host using the telnet protocol.
> More information: <https://manned.org/telnet>.

- Telnet to the default port of a host:

`telnet {{host}}`

- Telnet to a specific port of a host:

`telnet {{ip_address}} {{port}}`

- Exit a telnet session:

`quit`

- Emit the default escape character combination for terminating the session:

`Ctrl + ]`

- Start telnet with "x" as the session termination character:

`telnet -e {{x}} {{ip_address}} {{port}}`

- Telnet to Star Wars animation:

`telnet {{towel.blinkenlights.nl}}`
