# getmac 
## chatgpt 
The "getmac" command is used to display the media access control (MAC) address of a computer or network device. The MAC address is a unique hardware identifier assigned to each device on a network. 

When entering the command "getmac" in a Command Prompt window, the MAC addresses of all network devices connected to the computer will be displayed, along with their associated IP addresses and physical addresses. 

This information can be helpful for troubleshooting network issues, identifying devices on a network, and for security purposes. Additionally, the command can be modified to display specific information, such as the MAC address of a specific device using its IP address. 

Overall, the "getmac" command is a useful tool for network administrators and users who need to quickly identify the MAC addresses of network devices. 

## tldr 
 
> Display the MAC addresses of a system.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/getmac>.

- Display the MAC addresses for the current system:

`getmac`

- Display the details in a specific format:

`getmac /fo {{table|list|csv}}`

- Exclude the header in the output list:

`getmac /nh`

- Display the MAC addresses for a remote machine:

`getmac /s {{hostname}} /u {{username}} /p {{password}}`

- Display the MAC addresses with verbose information:

`getmac /v`

- Display detailed usage information:

`getmac /?`
