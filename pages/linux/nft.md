# nft 
## chatgpt 
nft is a command-line tool used for configuring and managing netfilter, the Linux kernel's firewall. Netfilter is a framework used for packet filtering and manipulation on Linux-based systems. nft allows administrators to create and modify firewall rules, manage network address translation (NAT), and filter packets based on various criteria.

The nft command can be used to perform a variety of tasks, including:

- Creating and modifying firewall rules: nft can be used to define rules for allowing or blocking traffic to and from specific IP addresses, ports, or protocols.
- Managing network address translation (NAT): nft can be used to modify the source and destination IP addresses and ports of packets passing through the firewall.
- Configuring logging: nft can be used to configure the firewall to log packets that match certain criteria, such as those that are blocked or allowed.
- Checking the status of the firewall: nft can be used to display the current firewall rules and their status.

Overall, the nft command provides administrators with powerful and flexible tools for configuring and managing the netfilter firewall on Linux-based systems. 

## tldr 
 
> Allows configuration of tables, chains and rules provided by the Linux kernel firewall.
> Nftables replaces iptables.
> More information: <https://wiki.nftables.org/wiki-nftables/index.php/Main_Page>.

- View current configuration:

`sudo nft list ruleset`

- Add a new table with family "inet" and table "filter":

`sudo nft add table {{inet}} {{filter}}`

- Add a new chain to accept all inbound traffic:

`sudo nft add chain {{inet}} {{filter}} {{input}} \{ type {{filter}} hook {{input}} priority {{0}} \; policy {{accept}} \}`

- Add a new rule to accept several TCP ports:

`sudo nft add rule {{inet}} {{filter}} {{input}} {{tcp}} {{dport \{ telnet, ssh, http, https \} accept}}`

- Add a NAT rule to translate all traffic from the `192.168.0.0/24` subnet to the host's public IP:

`sudo nft add rule {{nat}} {{postrouting}} ip saddr {{192.168.0.0/24}} {{masquerade}}`

- Show rule handles:

`sudo nft --handle --numeric list chain {{family}} {{table}} {{chain}}`

- Delete a rule:

`sudo nft delete rule {{inet}} {{filter}} {{input}} handle {{3}}`

- Save current configuration:

`sudo nft list ruleset > {{/etc/nftables.conf}}`
