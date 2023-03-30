# bmon 
## chatgpt 
The `bmon` command is used as a network bandwidth monitoring tool in Linux and Unix operating systems. It provides real-time monitoring of network traffic and displays various statistics about network usage, such as the amount of data transferred, packet counts, and network speed.

When the `bmon` command is executed, it starts monitoring the network interfaces on the system by default. You can specify which network interface(s) to monitor by passing the `-i` or `--interface` option followed by the interface name(s) as arguments.

The `bmon` command provides a simple console-based interface to display the network traffic statistics. The statistics are updated in real-time and can be displayed in various formats, including text and graphical. You can switch between different formats by pressing the `tab` key.

The `bmon` command supports various other options for customizing the monitoring settings and output formats. You can view the complete list of options and usage instructions by running the `bmon -h` command. 

## tldr 
 
> Monitor bandwidth and capture network related statistics.
> More information: <https://github.com/tgraf/bmon>.

- Display the list of all the interfaces:

`bmon -a`

- Display data transfer rates in bits per second:

`bmon -b`

- Set policy to define which network interface(s) is/are displayed:

`bmon -p {{interface_1,interface_2,interface_3}}`

- Set interval (in seconds) in which rate per counter is calculated:

`bmon -R {{2.0}}`
