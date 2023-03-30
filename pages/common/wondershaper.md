# wondershaper 
## chatgpt 
Wondershaper is a Linux command line tool used to manage and limit the bandwidth of network interfaces. The command is used to configure the bandwidth or traffic shaping policies on a network interface by setting the maximum upload and download speeds of that interface.

The command is typically used in situations where bandwidth is limited, and network traffic needs to be prioritized to avoid congestion. Wondershaper can be used to configure the upload and download speeds of individual applications or installments on a network.

The basic syntax of the command is: 

`wondershaper [interface] [downlink speed] [uplink speed]`

Where "interface" is the name of the network interface you want to limit the bandwidth to, "downlink speed" is the maximum download speed you want to allow (in kilobits per second), and "uplink speed" is the maximum upload speed you want to allow (in kilobits per second).

For example, to limit the bandwidth of the eth0 network interface to 500 kbps download and 100 kbps upload speeds, you would use the following command:

`sudo wondershaper eth0 500 100`

Once the command is executed, the bandwidth limit will be in effect until it is changed again or until the system is rebooted.

Overall, the wondershaper command is a powerful tool for tuning network performance and optimizing bandwidth usage on Linux systems. 

## tldr 
 
> Allows the user to limit the bandwidth of one or more network adapters.
> More information: <https://github.com/magnific0/wondershaper#usage>.

- Display [h]elp:

`wondershaper -h`

- Show the current [s]tatus of a specific [a]dapter:

`wondershaper -s -a {{adapter_name}}`

- Clear limits from a specific [a]dapter:

`wondershaper -c -a {{adapter_name}}`

- Set a specific maximum [d]ownload rate (in Kbps):

`wondershaper -a {{adapter_name}} -d {{1024}}`

- Set a specific maximum [u]pload rate (in Kbps):

`wondershaper -a {{adapter_name}} -u {{512}}`

- Set a specific maximum [d]ownload rate and [u]pload rate (in Kpbs):

`wondershaper -a {{adapter_name}} -d {{1024}} -u {{512}}`
