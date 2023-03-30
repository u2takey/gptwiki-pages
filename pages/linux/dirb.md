# dirb 
## chatgpt 
Dirb is a command-line tool commonly used by ethical hackers for web application scanning. When executed, dirb scans a website or a specific URL to find directories and files that may be useful for further testing.

The syntax for dirb is as follows:

`dirb <URL> <wordlist>`

- `URL`: The target website or URL to be scanned.
- `wordlist`: The list of words, also known as a dictionary, that dirb uses to brute-force scan and locate hidden files, directories, and folders on the web server.

Dirb performs a series of HTTP requests to the server, sending various GET and HEAD requests with different directory names appended to the base URL. If a 200 OK response is returned by the server, it means that the directory or file exists and is accessible. Dirb then records this information in its output.

Here is an example of the dirb command:

`dirb https://example.com/ /usr/share/wordlists/dirb/common.txt`

This command will scan https://example.com/ with the common.txt wordlist file located in /usr/share/wordlists/dirb/ directory.

Dirb is a useful tool for identifying known directories or files that might have been forgotten by a web developer or left unprotected by accident. However, it can also be misused in hacking attempts, so it's essential to use dirb only on websites or systems that one has permission to test. 

## tldr 
 
> Scan HTTP-based webservers for directories and files.
> More information: <http://dirb.sourceforge.net>.

- Scan a webserver using the default wordlist:

`dirb {{https://example.org}}`

- Scan a webserver using a custom wordlist:

`dirb {{https://example.org}} {{path/to/wordlist.txt}}`

- Scan a webserver non-recursively:

`dirb {{https://example.org}} -r`

- Scan a webserver using a specified user-agent and cookie for HTTP-requests:

`dirb {{https://example.org}} -a {{user_agent_string}} -c {{cookie_string}}`
