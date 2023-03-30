# feroxbuster 
## chatgpt 
Feroxbuster is a command-line tool designed for directory and content discovery on web applications. The name comes from the word "ferox," which is Latin for "wild" or "savage," indicating the tool's aptitude for uncovering information that might otherwise be hidden.

The tool was developed primarily for penetration testers, bug bounty hunters, and cybersecurity researchers who want to explore web applications for potential vulnerabilities or misconfigurations. Feroxbuster can be used to brute force, fuzz, and scan web servers or directories, and can easily integrate with other security tools such as Burp Suite, OWASP-ZAP, and Nmap.

Some of the key features of Feroxbuster include:

1. Directory bruteforce: Discover hidden directories and subdomains on web servers
2. Content discovery: Identify files and directories that are publicly available on web servers
3. Customizable wordlists: Feroxbuster comes with built-in wordlists, but users can also create their own
4. Recursive scanning: Can scan all subdirectories of the target URL
5. HTTP authentication support

In summary, Feroxbuster is a powerful and versatile command-line tool for web application security testing, and its various features make it a valuable asset for cybersecurity professionals. 

## tldr 
 
> Simple, fast, recursive content discovery tool written in Rust.
> Used to brute-force hidden paths on web servers and more.
> More information: <https://epi052.github.io/feroxbuster-docs/docs/>.

- Discover specific directories and files that match in the wordlist with extensions and 100 threads and a random user-agent:

`feroxbuster --url "{{https://example.com}}" --wordlist {{path/to/file}} --threads {{100}} --extensions "{{php,txt}}" --random-agent`

- Enumerate directories without recursion through a specific proxy:

`feroxbuster --url "{{https://example.com}}" --wordlist {{path/to/file}} --no-recursion --proxy "{{http://127.0.0.1:8080}}"`

- Find links in webpages:

`feroxbuster --url "{{https://example.com}}" --extract-links`

- Filter by a specific status code and a number of chars:

`feroxbuster --url "{{https://example.com}}" --filter-status {{301}} --filter-size {{4092}}`
