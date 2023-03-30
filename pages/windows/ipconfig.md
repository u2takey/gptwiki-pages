# ipconfig 
## chatgpt 
The "ipconfig" command in Windows is used to display network configuration information for the computer's currently active network cards. Here is a breakdown of each option and what it displays:

- "ipconfig /all" displays detailed information about all network connections, including IP addresses, subnet masks, default gateways, DNS servers, and more.

- "ipconfig /release" releases the IP address assigned to the computer by the DHCP server.

- "ipconfig /renew" requests a new IP address from the DHCP server.

- "ipconfig /flushdns" clears the DNS cache, which can resolve issues with domain name resolution.

- "ipconfig /displaydns" displays the contents of the DNS resolver cache.

- "ipconfig /registerdns" re-registers the computer's DNS name with the DNS server.

Note that in order to use these commands, you must open a command prompt window on your computer. To do this, press the Windows key + R, type "cmd" into the Run dialog box, and press Enter. Once the command prompt window opens, you can enter any of the "ipconfig" commands listed above. 

## tldr 
 
> Display and manage the network configuration of Windows.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/ipconfig>.

- Show a list of network adapters:

`ipconfig`

- Show a detailed list of network adapters:

`ipconfig /all`

- Renew the IP addresses for a network adapter:

`ipconfig /renew {{adapter}}`

- Free up the IP addresses for a network adapter:

`ipconfig /release {{adapter}}`

- Remove all data from the DNS cache:

`ipconfig /flushdns`
