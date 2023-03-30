# qrcp 
## chatgpt 
qrcp (Quick Remote Copy) is a command-line utility that allows you to transfer files over Wi-Fi between a computer and a mobile device or vice versa. Here is an overview of the command:

Syntax:
qrcp [options] [source] [destination]

Options:
-6, --ipv6: use IPV6 address
-a, --address <ip>: specify IP address to bind to
-c, --clipboard: send the file to the clipboard instead of saving it
-f, --force: overwrite existing files without prompting
-h, --help: display the help message
-i, --interface <device>: specify the network interface to use
-l, --list: list available network interfaces
-p, --port <number>: specify the port number
-s, --ssl: use HTTPS connection
-t, --trust: trust all devices without prompting
-v, --version: display the version number

Arguments:
source: the file or directory you want to transfer
destination: the destination directory on the mobile device or computer

Examples:

1. To transfer a file from the local computer to a mobile device, run the following command:

qrcp file.txt 192.168.0.10:/sdcard/Documents/

This will transfer the file "file.txt" to the mobile device located at IP address 192.168.0.10 and save it under the "Documents" directory on the SD card.

2. To transfer a file from a mobile device to a local computer, run the following command:

qrcp 192.168.0.10:/sdcard/Pictures/pic.jpg /home/user/Pictures/

This will transfer the file "pic.jpg" from the mobile device located at IP address 192.168.0.10 and save it in the "Pictures" directory on the local computer.

3. To list available network interfaces, run the following command:

qrcp -l

This will display a list of all available network interfaces on the local computer.

Overall, qrcp is a simple and convenient command-line tool for transferring files between a computer and a mobile device over a Wi-Fi network. 

## tldr 
 
> A file transfer tool.
> More information: <https://github.com/claudiodangelis/qrcp>.

- Send a file or directories:

`qrcp send {{path/to/file_or_directory path/to/file_directory ...}}`

- Receive files:

`qrcp receive`

- Compress content before transferring:

`qrcp send --zip {{path/to/file_or_directory}}`

- Specify a [p]ort to use:

`qrcp {{send|receive}} --port {{port_number}}`

- Specify the network [i]nterface to use:

`qrcp {{send|receive}} --interface interface`

- Keep the server alive:

`qrcp {{send|receive}} --keep-alive`
