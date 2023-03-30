# sublist3r 
## chatgpt 
Sublist3r is an open-source tool that helps in enumerating subdomains of given domain names using various search engines like Google, Bing, Yahoo, etc.

The command to use Sublist3r is as follows:

`sublist3r -d <domain-name>`

In the above command, "-d" is used to specify the domain name for which we want to list subdomains.

Sublist3r can also accept multiple domain names for enumeration by separating them with commas or specifying a file name that contains a list of domains.

Other optional flags that can be used with the Sublist3r command are:

- -v: verbose mode that displays additional information
- -t <threads>: specify the number of threads to be used for gathering subdomains (default is 10)
- -o <output-file>: specify the output file name for saving the results

Once the Sublist3r tool starts running, it queries the search engines for subdomains associated with the specified domain name and returns the results in the terminal or the specified output file. The output of Sublist3r typically includes the subdomain name, IP address, and the source search engine. 

Overall, Sublist3r is a useful tool for reconnaissance and helps in discovering potential attack surfaces that can be used for penetration testing or bug bounty assessment. 

## tldr 
 
> Fast subdomains enumeration tool for penetration testers.
> More information: <https://github.com/aboul3la/Sublist3r>.

- Find subdomains for a domain:

`sublist3r --domain {{domain_name}}`

- Find subdomains for a domain, also enabling brute force search:

`sublist3r --domain {{domain_name}} --bruteforce`

- Save the found subdomains to a text file:

`sublist3r --domain {{domain_name}} --output {{path/to/output_file}}`

- Output all available options:

`sublist3r --help`
