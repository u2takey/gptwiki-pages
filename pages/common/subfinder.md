# subfinder 
## chatgpt 
Subfinder is a popular command line tool used for enumerating subdomains. Essentially, it allows you to quickly find all subdomains for a particular domain name. When you run the subfinder command, it will use a variety of methods and techniques to search for subdomains associated with the domain name you provide. 

Subfinder can be a very useful tool for cybersecurity professionals, digital forensics investigators, and anyone else who needs to quickly gather subdomain information.

Here are some of the main features of subfinder:

- Multiple search options: subfinder offers several different methods for searching for subdomains, including recursive brute force searching, active subdomain scanning and subdomain discovery through various search engines, APIs, and scrapers. This makes it a versatile tool for different scenarios.
- Lightweight and fast: subfinder is designed to be lightweight and fast, allowing you to quickly scan large numbers of domains and subdomains without bogging down your system.
- Extensible: subfinder is built to be extensible, which means you can add your own sources to search or build your own plugins to customize how subdomains are found.

Overall, if you need to quickly gather subdomain information for a particular domain, subfinder is an excellent tool to consider. 

## tldr 
 
> A subdomain discovery tool that discovers valid subdomains for websites.
> Designed as a passive framework to be useful for bug bounties and safe for penetration testing.
> More information: <https://github.com/subfinder/subfinder>.

- Find subdomains for a specific domain:

`subfinder -d {{example.com}}`

- Show only the subdomains found:

`subfinder --silent -d {{example.com}}`

- Use a brute-force attack to find subdomains:

`subfinder -d {{example.com}} -b`

- Remove wildcard subdomains:

`subfinder -nW -d {{example.com}}`

- Use a given comma-separated list of resolvers:

`subfinder -r {{8.8.8.8}},{{1.1.1.1}} -d {{example.com}}`
