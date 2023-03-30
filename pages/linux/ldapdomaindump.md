# ldapdomaindump 
## chatgpt 
As an AI language model, I don't have actual access to a terminal nor execute commands in a computer outside of this environment. But I could provide you with the following general explanation:

ldapdomaindump is a command line tool that is used to dump the data or information stored within a domain's Lightweight Directory Access Protocol (LDAP) service. LDAP is a directory service protocol that is used to store and retrieve information in a hierarchical structure. The tool allows you to extract information from an LDAP server by making requests for the data stored in it.

When you run the ldapdomaindump command, it queries the LDAP server and returns information about the domain, its users, groups, and other objects. It can be useful for extracting information from an LDAP server for audit or forensic purposes or for troubleshooting LDAP-related issues.

To use the ldapdomaindump command, you need to have access to an LDAP server, and you need to provide the appropriate parameters, such as the server address, port number, login credentials, and other options. Once you have configured the command, you can run it to start extracting data from the target LDAP server.

It's worth noting that the ldapdomaindump tool can be used for both legitimate and malicious purposes, so it's important to use it responsibly and only with proper authorization. 

## tldr 
 
> Dump users, computers, groups, OS and membership information via LDAP to HTML, JSON and greppable output.
> See also `ldapsearch`.
> More information: <https://github.com/dirkjanm/ldapdomaindump>.

- Dump all information using the given LDAP account:

`ldapdomaindump --user {{domain}}\\{{administrator}} --password {{password|ntlm_hash}} {{hostname|ip}}`

- Dump all information, resolving computer hostnames:

`ldapdomaindump --resolve --user {{domain}}\\{{administrator}} --password {{password}} {{hostname|ip}}`

- Dump all information, resolving computer hostnames with the selected DNS server:

`ldapdomaindump --resolve --dns-server {{domain_controller_ip}} --user {{domain}}\\{{administrator}} --password {{password}} {{hostname|ip}}`

- Dump all information to the given directory without JSON output:

`ldapdomaindump --no-json --outdir {{path/to/directory}} --user {{domain}}\\{{administrator}} --password {{password}} {{hostname|ip}}`
