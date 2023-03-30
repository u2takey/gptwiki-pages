# iptables 
## chatgpt 
Iptables is a Linux command-line utility that allows system administrators to configure the built-in firewall (netfilter) that protects the system against network-based attacks. 

The iptables command allows users to create, modify or delete firewall rules, which define how incoming and outgoing network traffic should be filtered. Firewall rules are typically based on various criteria such as IP addresses, protocols, ports, interfaces, and more.

The basic syntax of the iptables command includes several parameters such as "-A" (append), "-I" (insert), "-D" (delete), "-P" (policy), and more, which are followed by the table name, chain name, and the rule specification. 

Here are some common iptables commands:

- **iptables -L**: List all the current firewall rules, including the default policy for each chain. 

- **iptables -F**: Flush all the current firewall rules, effectively disabling the firewall. 

- **iptables -A INPUT -p tcp --dport 22 -j ACCEPT**: Allow incoming SSH (Secure Shell) connections from any IP address by adding a new rule to the INPUT chain that matches the TCP protocol on port 22 and sets the action to ACCEPT.

- **iptables -A OUTPUT -d 192.168.1.0/24 -j DROP**: Drop all outgoing packets destined for the 192.168.1.0/24 network by adding a new rule to the OUTPUT chain that matches the destination IP address and sets the action to DROP.

- **iptables-save > /etc/sysconfig/iptables**: Save the current firewall rules to a file for persistent storage across system reboots.

Overall, iptables is a powerful tool for securing a Linux system from potential network-based threats, but it requires careful planning and understanding to avoid any unintended consequences. 

## tldr 
 
> Program that allows configuration of tables, chains and rules provided by the Linux kernel firewall.
> More information: <https://www.netfilter.org/projects/iptables/>.

- View chains, rules, and packet/byte counters for the filter table:

`sudo iptables -vnL`

- Set chain policy rule:

`sudo iptables -P {{chain}} {{rule}}`

- Append rule to chain policy for IP:

`sudo iptables -A {{chain}} -s {{ip}} -j {{rule}}`

- Append rule to chain policy for IP considering protocol and port:

`sudo iptables -A {{chain}} -s {{ip}} -p {{protocol}} --dport {{port}} -j {{rule}}`

- Add a NAT rule to translate all traffic from the `192.168.0.0/24` subnet to the host's public IP:

`sudo iptables -t {{nat}} -A {{POSTROUTING}} -s {{192.168.0.0/24}} -j {{MASQUERADE}}`

- Delete chain rule:

`sudo iptables -D {{chain}} {{rule_line_number}}`

- Save iptables configuration of a given table to a file:

`sudo iptables-save -t {{tablename}} > {{path/to/iptables_file}}`

- Restore iptables configuration from a file:

`sudo iptables-restore < {{path/to/iptables_file}}`
