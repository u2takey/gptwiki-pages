# tftp 
## chatgpt 
The tftp command is a simple file transfer protocol that is used to transfer files between two networked devices. It stands for Trivial File Transfer Protocol. The command is used to initiate and control file transfers using the TFTP protocol. 

Here are some of the basic features of the TFTP command:

1. Simple: TFTP is a very simple protocol, making it easy to use and implement.

2. UDP-based: TFTP uses User Datagram Protocol (UDP) to transfer files.

3. No built-in security: TFTP does not provide any security features and sends files unencrypted.

4. Does not require authentication: TFTP does not require authentication during file transfer.

5. Limited functionality: TFTP supports only basic file transfer functions.

The TFTP command is used between two devices on the same network. The client device sends a request to a TFTP server to initiate a file transfer. The TFTP server responds and then begins transferring the requested file. The client device receives the file and saves it to the specified location.

To use the TFTP command, you need to know the IP address of the TFTP server and the file name you want to transfer. Here is an example of how to use the TFTP command:

tftp 192.168.0.10 -c get myfile.txt

In this example, the command is used to download the file myfile.txt from the TFTP server at the IP address 192.168.0.10. The -c option specifies that the TFTP client should connect to the server, and the get command tells the server to send the specified file to the client.

Overall, the TFTP command is a useful tool for transferring files between devices on the same network. However, it should be used carefully, as it does not provide any security or authentication features. 

## tldr 
 
> Trivial File Transfer Protocol client.
> More information: <https://manned.org/tftp.1>.

- Connect to a TFTP server specifying its IP address and port:

`tftp {{server_ip}} {{port}}`

- Connect to a TFTP server and execute a TFTP [c]ommand:

`tftp {{server_ip}} -c {{command}}`

- Connect to a TFTP server using IPv6 and force originating port to be in [R]ange:

`tftp {{server_ip}} -6 -R {{port}}:{{port}}`

- Set the transfer mode to binary or ascii through the tftp client:

`mode {{binary|ascii}}`

- Download file from a server through the tftp client:

`get {{file}}`

- Upload file to a server through the tftp client:

`put {{file}}`

- Exit the tftp client:

`quit`
