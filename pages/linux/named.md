# named 
## chatgpt 
The "named" command is used to start the BIND (Berkeley Internet Name Domain) domain name server. BIND is an open-source software that provides domain name resolution on the internet. The named command is used to initiate the server daemon, which will then listen for incoming DNS queries and provide authoritative responses to the client.

When used with the appropriate options and configuration files, the named command can be used to create a DNS server that can provide name resolution services to internet-connected hosts. A number of configuration files are required to set up a BIND server, including options file, named.conf file, and zone files, which contain authoritative information for a particular domain.

The named command is typically run as a background service, started either manually or on system boot. Once running, it will listen for incoming DNS requests, process them, and return a response to the client. If any errors or configuration issues are encountered, they can be monitored using logging facilities provided by BIND. 

## tldr 
 
> Execute the DNS (Dynamic Name Service) server daemon that converts host names to IP addresses and vice versa.
> More information: <https://manned.org/named>.

- Read the default configuration file `/etc/named.conf`, read any initial data and listen for queries:

`named`

- Read a custom configuration file:

`named -c {{path/to/named.conf}}`

- Use IPv4 or IPv6 only, even if the host machine is capable of utilising other protocols:

`named {{-4|-6}}`

- Listen for queries on a specific port instead of the default port 53:

`named -p {{port}}`

- Run the server in the foreground and do not daemonize:

`named -f`
