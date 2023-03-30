# amass intel 
## chatgpt 
The command "amass intel" is related to the Amass tool, which is a reconnaissance and enumeration tool used for information gathering and asset discovery. 

When you run "amass intel" command, it is telling the Amass tool to start the intelligence gathering process. This process involves scanning target networks, domains, and IP addresses to gather information, such as subdomains, web pages, IP addresses, email addresses, and other relevant data, about the target.

The "amass intel" command can be further customized with different flags and options, depending on the desired level of detail and scope for the intelligence gathering process. Some of the options that can be included in the command are:

- -active: discovers active network assets that are currently online
- -passive: performs passive reconnaissance, without actively scanning the target network
- -brute: performs brute-force attacks to identify subdomains and domain names
- -whois: performs a WHOIS lookup to retrieve registration information about the target domain
- -port: scans specific ports to identify open services and vulnerabilities

Overall, the "amass intel" command is a powerful tool for reconnaissance and enumeration activities, which can help to identify potential vulnerabilities and security risks in target networks, domains, and IP addresses. 

## tldr 
 
> Collect open source intel on an organisation like root domains and ASNs.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-intel-subcommand>.

- Find root domains in an IP address range:

`amass intel -addr {{192.168.0.1-254}}`

- Use active recon methods:

`amass intel -active -addr {{192.168.0.1-254}}`

- Find root domains related to a domain:

`amass intel -whois -d {{domain_name}}`

- Find ASNs belonging to an organisation:

`amass intel -org {{organisation_name}}`

- Find root domains belonging to a given Autonomous System Number:

`amass intel -asn {{asn}}`

- Save results to a text file:

`amass intel -o {{output_file}} -whois -d {{domain_name}}`
