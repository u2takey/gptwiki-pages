# firewall-cmd 
## chatgpt 
firewall-cmd is a command-line utility for managing the firewall configuration on Linux operating systems. It is used to open or close ports, allow or deny traffic, and manage firewalld services.

The firewall-cmd command has several options and subcommands that can be used to manage the firewall configuration. Some of the common options and subcommands are:

- --list-services: Lists the currently configured services and ports that are allowed through the firewall.
- --add-service: Adds a service to the list of allowed services and opens the required ports for that service.
- --remove-service: Removes a service from the list of allowed services and closes the ports for that service.
- --add-port: Adds a port to the list of allowed ports and opens that port for traffic.
- --remove-port: Removes a port from the list of allowed ports and closes that port for traffic.
- --zone: Specifies the firewall zone to which the firewall rules should be applied.
- --permanent: Indicates that the changes made to the firewall should be permanent and persist across reboots.

Overall, firewall-cmd is a powerful tool that can be used to configure and manage the firewall on Linux systems, thereby enhancing the security of these systems. 

## tldr 
 
> The firewalld command-line client.
> More information: <https://firewalld.org/documentation/man-pages/firewall-cmd>.

- View the available firewall zones:

`firewall-cmd --get-active-zones`

- View the rules which are currently applied:

`firewall-cmd --list-all`

- Permanently move the interface into the block zone, effectively blocking all communication:

`firewall-cmd --permanent --zone={{block}} --change-interface={{enp1s0}}`

- Permanently open the port for a service in the specified zone (like port 443 when in the `public` zone):

`firewall-cmd --permanent --zone={{public}} --add-service={{https}}`

- Permanently close the port for a service in the specified zone (like port 80 when in the `public` zone):

`firewall-cmd --permanent --zone={{public}} --remove-service={{http}}`

- Permanently open two arbitrary ports in the specified zone:

`firewall-cmd --permanent --zone={{public}} --add-port={{25565/tcp}} --add-port={{19132/udp}}`

- Reload firewalld to force rule changes to take effect:

`firewall-cmd --reload`
