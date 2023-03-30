# ethtool 
## chatgpt 
`ethtool` is a Linux command-line tool used to query and control network interface settings, drivers, and hardware. 

The basic syntax of the ethtool command is:

```sh
ethtool [options] [device]
```

Where:
- `options` are various command flags, such as `-i` for device driver information, `-g` for ring buffer, and so on
- `device` is the name of the ethernet device you want to list or modify settings for, such as `eth0` or `enp3s0` (device name may vary depending on your system).

Some common options of `ethtool` command include:

- `-i`: Display device driver information
- `-s`: Set various network interface parameters
- `-a`: Display or set adaptive settings 
- `-g`: Query the kernel for the number of ring buffer descriptors for a device
- `-p`: Blink the LED on a specified ethernet device for identification purposes
- `-S`: Display hardware offload statistics for the network interface

Overall, the `ethtool` command is a powerful command-line tool for managing and diagnosing network interface configuration and performance on Linux systems. 

## tldr 
 
> Display and modify Network Interface Controller (NIC) parameters.
> More information: <http://man7.org/linux/man-pages/man8/ethtool.8.html>.

- Display the current settings for an interface:

`ethtool {{eth0}}`

- Display the driver information for an interface:

`ethtool --driver {{eth0}}`

- Display all supported features for an interface:

`ethtool --show-features {{eth0}}`

- Display the network usage statistics for an interface:

`ethtool --statistics {{eth0}}`

- Blink one or more LEDs on an interface for 10 seconds:

`ethtool --identify {{eth0}} {{10}}`

- Set the link speed, duplex mode, and parameter auto-negotiation for a given interface:

`ethtool -s {{eth0}} speed {{10|100|1000}} duplex {{half|full}} autoneg {{on|off}}`
