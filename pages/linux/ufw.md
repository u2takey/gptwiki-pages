# ufw 
## chatgpt 
ufw stands for Uncomplicated Firewall. It is a command line tool used in Ubuntu and other Linux distributions to manage the firewall rules. 

The ufw command allows users to enable or disable the firewall, add or remove rules, and check the status of the firewall. The firewall blocks incoming and outgoing traffic based on predefined rules. 

Some examples of ufw commands are:
- ufw enable: Enables the firewall
- ufw disable: Disables the firewall
- ufw status: Shows the current status of the firewall and the active rules
- ufw allow <port>/tcp: Allows incoming traffic on a specific TCP port
- ufw deny <port>/tcp: Denies incoming traffic on a specific TCP port
- ufw reset: Resets the firewall configuration to the default settings

The ufw command can be used by system administrators to secure their servers by blocking unauthorized access to the network. It is an essential tool for improving the security of your system. 

## tldr 
 
> Uncomplicated Firewall.
> Frontend for iptables aiming to make configuration of a firewall easier.
> More information: <https://wiki.ubuntu.com/UncomplicatedFirewall>.

- Enable ufw:

`ufw enable`

- Disable ufw:

`ufw disable`

- Show ufw rules, along with their numbers:

`ufw status numbered`

- Allow incoming traffic on port 5432 on this host with a comment identifying the service:

`ufw allow {{5432}} comment "{{Service}}"`

- Allow only TCP traffic from 192.168.0.4 to any address on this host, on port 22:

`ufw allow proto {{tcp}} from {{192.168.0.4}} to {{any}} port {{22}}`

- Deny traffic on port 80 on this host:

`ufw deny {{80}}`

- Deny all UDP traffic to ports in range 8412:8500:

`ufw deny proto {{udp}} from {{any}} to {{any}} port {{8412:8500}}`

- Delete a particular rule. The rule number can be retrieved from the `ufw status numbered` command:

`ufw delete {{rule_number}}`
