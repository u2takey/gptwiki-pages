# resolvectl 
## chatgpt 
resolvectl is a command-line tool that is used to manage the DNS resolver configuration on Linux systems. It allows users to view and modify the contents of the /etc/resolv.conf file, which contains the DNS configuration information for the system.

When run without any arguments, resolvectl displays the current DNS resolver configuration. This includes the currently used DNS servers, search domains, and other options. The output provides useful information about how the system is resolving domain names.

Users can modify the DNS resolver configuration using the resolvectl command. For example, to add a DNS server, the following command can be used:

resolvectl dns eth0 8.8.8.8 

This will add the Google DNS server (8.8.8.8) to the DNS server list for the network interface 'eth0'. To remove a DNS server, the following command can be used:

resolvectl dns-down eth0 8.8.8.8 

This will remove the Google DNS server from the DNS server list for the network interface 'eth0'.

Other options for resolvectl include the ability to modify the search domains, set the DNS search order, and enforce DNSSEC validation. For more information about the different options available with resolvectl, users can refer to the man pages or online documentation. 

## tldr 
 
> Resolve domain names, IPV4 and IPv6 addresses, DNS resource records, and services.
> Introspect and reconfigure the DNS resolver.
> More information: <https://www.freedesktop.org/software/systemd/man/resolvectl.html>.

- Show DNS settings:

`resolvectl status`

- Resolve the IPv4 and IPv6 addresses for one or more domains:

`resolvectl query {{domain1 domain2 ...}}`

- Retrieve the domain of a specified IP:

`resolvectl query {{ip_address}}`

- Retrieve an MX record of domain:

`resolvectl --legend={{no}} --type={{MX}} query {{domain}}`

- Resolve an SRV record, for example _xmpp-server._tcp gmail.com:

`resolvectl service _{{service}}._{{protocol}} {{name}}`

- Retrieve the public key from an email address from an OPENPGPKEY DNS record:

`resolvectl opengpg {{email}}`

- Retrieve a TLS key:

`resolvectl tlsa tcp {{domain}}:443`
