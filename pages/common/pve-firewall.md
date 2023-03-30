# pve-firewall 
## chatgpt 
As an AI language model, I assume that the command "pve-firewall" refers to the Proxmox Virtual Environment (PVE) firewall utility command, which is used in PVE to manage the firewall rules and configurations. 

The "pve-firewall" command allows system administrators to configure and manage the firewall settings of their PVE server. The command provides various options to define firewall rules, enable/disable or list configured rules, configure network interfaces, and manage source or destination IP or MAC addresses.

Some key options available with the "pve-firewall" command are:

- `list` : This option is used to display the list of configured firewall rules or elements. 
- `add` : Used to create and add a new firewall rule or modify an existing one. Users can specify a set of rules, action types (accept, reject, or drop), or a group of IP or MAC addresses, and other settings. 
- `delete` : Used to remove the firewall rule or element. Users can specify a rule ID or name to delete. 
- `enable` or `disable`: Used to enable or disable the firewall service. 

Overall, the "pve-firewall" command is a powerful tool that allows system administrators to configure custom firewall rules and settings to protect their PVE server from unauthorized access and malicious attacks. 

## tldr 
 
> Manage Proxmox VE Firewall.
> More information: <https://pve.proxmox.com/wiki/Firewall>.

- Compile and print all firewall rules:

`pve-firewall compile`

- Show information about the local network:

`pve-firewall localnet`

- Restart the Proxmox VE Firewall service:

`pve-firewall restart`

- Start the Proxmox VE Firewall service:

`pve-firewall start`

- Stop the Proxmox VE Firewall service:

`pve-firewall stop`

- Simulate all firewall rules:

`pve-firewall simulate`

- Show the status of Proxmox VE Firewall:

`pve-firewall status`
