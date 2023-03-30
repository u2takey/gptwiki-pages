# ifconfig 
## chatgpt 
ifconfig is a command-line utility used in Unix-based operating systems such as Linux, macOS, and BSD to view and configure network interfaces. Its name is short for "interface configuration".

When executed, the ifconfig command displays information about all the network interfaces on the computer. This information includes the interface name, hardware address (also known as the MAC address), IP address, subnet mask, and various other attributes, such as MTU (Maximum Transmission Unit) and link status.

In addition to displaying information, you can also use the ifconfig command to configure network interfaces. For example, you can set the IP address and subnet mask of an interface, enable or disable the interface, or configure advanced settings such as the number of packet retries.

The syntax of the ifconfig command is as follows:

ifconfig [interface] [options]

Here, "interface" refers to the name or identifier of the network interface you want to configure, such as eth0 or wlan0. Options include various parameters that allow you to configure the interface, such as setting the IP address or subnet mask.

Some examples of how to use the ifconfig command include:

- View information about the network interfaces: `ifconfig`
- View detailed information about a specific interface: `ifconfig eth0`
- Configure the IP address of an interface: `sudo ifconfig eth0 192.168.1.100`
- Enable or disable an interface: `sudo ifconfig eth0 up` or `sudo ifconfig eth0 down` 

## tldr 
 
> Network Interface Configurator.
> More information: <https://net-tools.sourceforge.io/man/ifconfig.8.html>.

- View network settings of an Ethernet adapter:

`ifconfig eth0`

- Display details of all interfaces, including disabled interfaces:

`ifconfig -a`

- Disable eth0 interface:

`ifconfig eth0 down`

- Enable eth0 interface:

`ifconfig eth0 up`

- Assign IP address to eth0 interface:

`ifconfig eth0 {{ip_address}}`
