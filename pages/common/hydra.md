# hydra 
## chatgpt 
Hydra is a password cracking tool that can be used to perform brute-force attacks to crack passwords of various online platforms, such as email, FTP, SSH, and HTTP. 

The syntax of the basic command for Hydra is:
hydra <target> <protocol> <options>

Here is what each part of the command means:

- `<target>`: This is the target system or platform that you want to attack. It can be an IP address, website URL, or hostname. 
- `<protocol>`: This is the protocol used by the target system. Hydra supports various protocols, such as FTP, SSH, Telnet, SMTP, SMB, HTTP, and many others. You need to specify the protocol in order for Hydra to use the correct method of attacking the target. 
- `<options>`: These are the options that you can use to customize your attack. They can include parameters such as the username list, password list, number of threads, output file, and more.

Here is an example command for an HTTP brute-force attack on a website:
hydra -l admin -P /path/to/password/list.txt example.com http-post-form "/login.php:user=^USER^&password=^PASS^:Invalid username or password"

This command will attack the website example.com using the HTTP protocol, and it will use the username "admin" and a password list located at "/path/to/password/list.txt". The hydra tool will send POST requests to the "/login.php" page and will replace the ^USER^ and ^PASS^ placeholders with usernames and passwords from the specified lists. If a username and password combination is accepted, the response will be "Invalid username or password". The "-l" option specifies the username list, while "-P" specifies the password list. The "http-post-form" option specifies the form data that needs to be submitted. 

Overall, Hydra is a powerful tool that can be used for ethical hacking, security testing, and penetration testing purposes. However, using it without proper authorization or legal permission is strictly prohibited. 

## tldr 
 
> Online password guessing tool.
> Protocols supported include FTP, HTTP(S), SMTP, SNMP, XMPP, SSH, and more.
> More information: <https://github.com/vanhauser-thc/thc-hydra>.

- Start Hydra's wizard:

`hydra-wizard`

- Guess SSH credentials using a given username and a list of passwords:

`hydra -l {{username}} -P {{path/to/wordlist.txt}} {{host_ip}} {{ssh}}`

- Guess HTTPS webform credentials using two specific lists of usernames and passwords ("https_post_request" can be like "username=^USER^&password=^PASS^"):

`hydra -L {{path/to/usernames.txt}} -P {{path/to/wordlist.txt}} {{host_ip}} {{https-post-form}} "{{url_without_host}}:{{https_post_request}}:{{login_failed_string}}"`

- Guess FTP credentials using usernames and passwords lists, specifying the number of threads:

`hydra -L {{path/to/usernames.txt}} -P {{path/to/wordlist.txt}} -t {{n_tasks}} {{host_ip}} {{ftp}}`

- Guess MySQL credentials using a username and a passwords list, exiting when a username/password pair is found:

`hydra -l {{username}} -P {{path/to/wordlist.txt}} -f {{host_ip}} {{mysql}}`

- Guess RDP credentials using a username and a passwords list, showing each attempt:

`hydra -l {{username}} -P {{path/to/wordlist.txt}} -V {{rdp://host_ip}}`

- Guess IMAP credentials on a range of hosts using a list of colon-separated username/password pairs:

`hydra -C {{path/to/username_password_pairs.txt}} {{imap://[host_range_cidr]}}`

- Guess POP3 credentials on a list of hosts using usernames and passwords lists, exiting when a username/password pair is found:

`hydra -L {{path/to/usernames.txt}} -P {{path/to/wordlist.txt}} -M {{path/to/hosts.txt}} -F {{pop3}}`
