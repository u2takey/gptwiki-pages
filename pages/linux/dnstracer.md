# dnstracer 
## chatgpt 
The command "dnstracer" is a command line tool that is used to trace the path that a DNS query follows from your computer to its final destination. It is a useful tool for diagnosing DNS related issues and for understanding how DNS resolution works.

Here is a breakdown of the command:

dnstracer - This is the name of the command that needs to be typed in the terminal to start the tool.

When running the dnstracer command, you need to specify a domain name for which you want to trace the DNS path. For example:

dnstracer example.com

The output of the command will include:

- The DNS servers that are responsible for resolving the domain.
- The IP addresses of the DNS servers.
- The response times of the DNS servers.
- The path that the DNS query took to reach the final DNS server.
- The final IP address that was returned by the DNS server.

Overall, dnstracer is a powerful tool for understanding how DNS resolution works and for diagnosing DNS-related issues. 

## tldr 
 
> The dnstracer command determines where a DNS gets its information from.
> More information: <https://manned.org/dnstracer>.

- Find out where your local DNS got the information on www.example.com:

`dnstracer {{www.example.com}}`

- Start with a [s]pecific DNS that you already know:

`dnstracer -s {{dns.example.org}} {{www.example.com}}`

- Only query IPv4 servers:

`dnstracer -4 {{www.example.com}}`

- Retry each request 5 times on failure:

`dnstracer -r {{5}} {{www.example.com}}`

- Display all steps during execution:

`dnstracer -v {{www.example.com}}`

- Display an [o]verview of all received answers after execution:

`dnstracer -o {{www.example.com}}`
