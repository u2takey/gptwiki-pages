# vnstati 
## chatgpt 
Vnstati is a command line tool for Linux that generates network traffic statistics in the form of PNG images. It measures different aspects of network traffic, such as total amount of data transmitted or received, the rate of data transferred, the types of traffic, and more. 

The basic syntax of the command is: 

```
vnstati [options] [interface] [output file]
```

The options parameter can be used to specify different types of statistics to be generated. Some of the commonly used options are:

- `-s`: display a summary of traffic statistics for each minute, hour or day
- `-h`: display hourly traffic statistics
- `-d`: display daily traffic statistics
- `-t`: display top 10 traffic sources and destinations
- `-p`: display the types of protocols used for network traffic

The interface parameter specifies the network interface to be monitored, such as eth0 or wlan0. The output file parameter specifies the name and location of the PNG file to be created.

For example, the following command will generate a PNG file showing a summary of network traffic statistics for the interface eth0:

```
vnstati -s -i eth0 -o /home/user/vnstati_summary.png
```

Overall, vnstati is a useful tool for monitoring and analyzing network traffic in Linux systems. It can help to identify any unusual activity or patterns in network usage and optimize network performance accordingly. 

## tldr 
 
> PNG image output support for vnStat.
> More information: <https://manned.org/vnstati>.

- Output a summary of the last 2: months, days, and all-time:

`vnstati --summary --iface {{network_interface}} --output {{path/to/output.png}}`

- Output the 10 most traffic-intensive days of all time:

`vnstati --top10 --iface {{network_interface}} --output {{path/to/output.png}}`

- Output monthly traffic statistics from the last 12 months:

`vnstati --months --iface {{network_interface}} --output {{path/to/output.png}}`

- Output hourly traffic statistics from the last 24 hours:

`vnstati --hours --iface {{network_interface}} --output {{path/to/output.png}}`
