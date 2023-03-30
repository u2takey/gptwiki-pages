# amass enum 
## chatgpt 
The "amass enum" command is used to run the enumeration phase of the Amass tool. Amass is an open-source tool used for mapping out a target's network infrastructure by discovering domains, subdomains, and IP addresses associated with the target. The "enum" part of the command stands for "enumeration", which is the process of identifying and listing all possible targets for analysis.

When the "amass enum" command is initiated, the tool will begin scanning the target's network and collecting as much data as possible on available domains, subdomains, and IP addresses associated with the target. This process may take some time, depending on the size of the target's infrastructure.

The output of the "amass enum" command includes information such as the discovered domains, subdomains, and IP addresses, as well as other relevant metadata such as associated subnets, services, and ports. This information can then be used for further analysis, including vulnerability assessments and penetration testing.

Overall, the "amass enum" command is a powerful tool for identifying potential targets on a network and is an essential part of many cybersecurity professionals' workflows. 

## tldr 
 
> Find subdomains of a domain.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-enum-subcommand>.

- Passively find subdomains of a domain:

`amass enum -passive -d {{domain_name}}`

- Find subdomains of a domain and actively verify them attempting to resolve the found subdomains:

`amass enum -active -d {{domain_name}} -p {{80,443,8080}}`

- Do a brute force search for subdomains:

`amass enum -brute -d {{domain_name}}`

- Save the results to a text file:

`amass enum -o {{output_file}} -d {{domain_name}}`

- Save the results to a database:

`amass enum -o {{output_file}} -dir {{path/to/database_directory}}`
