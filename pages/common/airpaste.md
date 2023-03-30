# airpaste 
## chatgpt 
Airpaste is a command-line tool that allows you to share data over the network through the terminal. It uses multicast DNS to discover peers and establishes a direct connection between them. 

Here's a breakdown of some common options and arguments you can use with the command:

- `airpaste send [file]`: Use this option to send a file to another device on the network. For example, `airpaste send image.jpg` will send the "image.jpg" file to any available peers. Once the transfer is complete, the receiving device will output the contents of the file to its terminal.

- `airpaste listen`: Use this option to listen for incoming data from other devices. It will display any received data in the terminal. You can't use this option to send data, but it's useful for receiving data from peers who are using the "airpaste send" command.

- `airpaste -h/--help`: Displays help information about the command, including a list of available options and arguments.

- `airpaste --version`: Displays the version number of the airpaste command.

Overall, airpaste is a handy tool for quickly sharing files and data between devices on the same network without the need for additional software or tools. 

## tldr 
 
> Share messages and files on the same network using mDNS.
> More information: <https://github.com/mafintosh/airpaste>.

- Wait for a message and display it when received:

`airpaste`

- Send text:

`echo {{text}} | airpaste`

- Send a file:

`airpaste < {{path/to/file}}`

- Receive a file:

`airpaste > {{path/to/file}}`

- Create or join a channel:

`airpaste {{channel_name}}`
