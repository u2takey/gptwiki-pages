# wpscan 
## chatgpt 
The `wpscan` command is a tool used to scan WordPress websites for vulnerabilities and potential security issues. It is a command-line utility that can be used to test the security of WordPress websites by scanning them for known vulnerabilities, weak passwords, and other security issues.

Some of the things that the `wpscan` command can do include:

- Checking for outdated versions of WordPress, plugins, and themes
- Checking for common vulnerabilities such as SQL injection and XSS exploits
- Brute-forcing logins with a list of possible usernames and passwords
- Enumerating user accounts on the site
- Gathering information about the site such as its version, installed plugins, and themes

Overall, the `wpscan` command is an essential tool for anyone who wants to ensure the security of their WordPress website. It can help identify vulnerabilities before they can be exploited by attackers, and can help website owners take the necessary steps to secure their site against potential threats. 

## tldr 
 
> WordPress vulnerability scanner.
> More information: <https://github.com/wpscanteam/wpscan>.

- Update the vulnerability database:

`wpscan --update`

- Scan a WordPress website:

`wpscan --url {{url}}`

- Scan a WordPress website, using random user agents and passive detection:

`wpscan --url {{url}} --stealthy`

- Scan a WordPress website, checking for vulnerable plugins and specifying the path to the `wp-content` directory:

`wpscan --url {{url}} --enumerate {{vp}} --wp-content-dir {{remote/path/to/wp-content}}`

- Scan a WordPress website through a proxy:

`wpscan --url {{url}} --proxy {{protocol://ip:port}} --proxy-auth {{username:password}}`

- Perform user identifiers enumeration on a WordPress website:

`wpscan --url {{url}} --enumerate {{u}}`

- Execute a password guessing attack on a WordPress website:

`wpscan --url {{url}} --usernames {{username|path/to/usernames.txt}} --passwords {{path/to/passwords.txt}} threads {{20}}`

- Scan a WordPress website, collecting vulnerability data from the WPVulnDB (https://wpvulndb.com/):

`wpscan --url {{url}} --api-token {{token}}`
