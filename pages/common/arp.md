# arp 
## chatgpt 
arp is a command used in computer networking to display or modify the Address Resolution Protocol (ARP) cache, which is a mapping between IP addresses and physical addresses (MAC addresses) for local network devices.

The basic syntax of the arp command is:

```
arp [-a] [-d] [-s] [hostname] [MAC_address]
```

Where: 

- `-a` – Displays the current ARP cache table for all network interfaces. 
- `-d` – Deletes a specific ARP cache entry. 
- `-s` – Adds a static ARP cache entry. This requires specifying the IP address and the associated MAC address. 
- `hostname` – Specifies the hostname or IP address of a remote computer to resolve and add to the cache. 
- `MAC_address` – Specifies the physical address of the host to add or remove from the cache. 

Here are some common uses of the arp command:

- To display the ARP cache table: 

  ```
  arp -a
  ```

- To display the ARP cache table for a specific interface:

  ```
  arp -a -i eth0
  ```

- To delete an entry from the ARP cache: 

  ```
  arp -d 192.168.1.1
  ```

- To add a static ARP entry: 

  ```
  arp -s 192.168.1.2 11:22:33:44:55:66
  ```

Overall, the arp command is a useful tool for diagnosing and troubleshooting network connectivity issues. 

## tldr 
 
> Show and manipulate your system's ARP cache.
> More information: <https://manned.org/arp>.

- Show the current ARP table:

`arp -a`

- Clear the entire cache:

`sudo arp -a -d`

- Delete a specific entry:

`arp -d {{address}}`

- Create an entry in the ARP table:

`arp -s {{address}} {{mac_address}}`
