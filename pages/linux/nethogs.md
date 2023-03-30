# nethogs 
## chatgpt 
Nethogs is a command-line tool used for monitoring network traffic by displaying bandwidth usage per process or per connection. It is helpful for network administrators to quickly identify the applications or processes that are using excessive network resources.

When you run the "nethogs" command, it will display a real-time view of network traffic by showing the process name, its PID (Process ID), sent/received data, and current transfer rate. By default, nethogs displays information for all network interfaces available on the system, but you can narrow down the results to a specific interface with the "-i" option.

Usage:

To use nethogs, simply open a terminal window and type "nethogs" followed by any options you want to use.

Examples:

1. To display real-time network traffic for all interfaces:

   nethogs

2. To monitor network traffic for a specific network interface (e.g. eth0):

   nethogs -i eth0

3. To run nethogs as root:

   sudo nethogs

Note: Running nethogs as root will display the traffic for all users and processes on the system. 

## tldr 
 
> Monitor bandwidth usage per process.
> More information: <https://github.com/raboof/nethogs>.

- Start nethogs as root (default device is eth0):

`sudo nethogs`

- Monitor bandwidth on specific device:

`sudo nethogs {{device}}`

- Monitor bandwidth on multiple devices:

`sudo nethogs {{device1}} {{device2}}`

- Specify refresh rate:

`sudo nethogs -t {{seconds}}`
