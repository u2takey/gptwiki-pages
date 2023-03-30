# ip rule 
## chatgpt 
The "ip rule" command in Linux systems is used to manage network routing rules. It allows the user to define policies and routing tables for network traffic. 

Here's a detailed explanation of the command:

- "ip" stands for "Internet Protocol" and is a command-line utility that allows the user to perform various tasks related to network configuration and management.
- "rule" is a subcommand under "ip" that is used to manage network routing rules. 
- When the "ip rule" command is run, it displays a list of rules that are currently defined on the system. These rules determine how packets are routed through the network.
- The output of the command shows each rule's priority, selector, and action. The priority is a number that determines the order in which rules are evaluated. The selector is a set of conditions that determines which packets match the rule, and the action is the routing table to which the packets are sent.
- The "ip rule" command can also be used to add, delete or modify network routing rules. For example, to add a new rule, you would specify the conditions that the rule should match and the action that should be taken for packets that match those conditions.
- The "ip rule" command is a powerful tool that can be used to manage complex network routing policies, such as load balancing and policy-based routing. However, it should be used with caution as incorrect configuration of rules can result in network connectivity issues. 

## tldr 
 
> IP routing policy database management.
> More information: <https://man7.org/linux/man-pages/man8/ip-rule.8.html>.

- Display the routing policy:

`ip rule {{show|list}}`

- Add a new rule based on packet source addresses:

`sudo ip rule add from {{192.168.178.2/32}}`

- Add a new rule based on packet destination addresses:

`sudo ip rule add to {{192.168.178.2/32}}`

- Delete a rule based on packet source addresses:

`sudo ip rule delete from {{192.168.178.2/32}}`

- Delete a rule based on packet destination addresses:

`sudo ip rule delete to {{192.168.178.2/32}}`

- Flush all deleted rules:

`ip rule flush`

- Save all rules to a file:

`ip rule save > {{path/to/ip_rules.dat}}`

- Restore all rules from a file:

`ip rule restore < {{path/to/ip_rules.dat}}`
