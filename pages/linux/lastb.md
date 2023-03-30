# lastb 
## chatgpt 
The `lastb` command is used in Linux and Unix-based operating systems to view a log of unsuccessful login attempts. The "b" in `lastb` stands for "bad" or "failed" attempts.

When the command is executed, it reads from the `/var/log/btmp` file and presents a list of all users who attempted to log in but failed, along with the IP address and timestamp of the attempts. It provides details such as the attempted usernames, source of the attempted login, and the time of the attempt.

This command can be useful for identifying potential security breaches or unauthorized access attempts to your system. By analyzing the output of `lastb`, system administrators can take appropriate action to improve the security of the system such as disabling compromised accounts, blocking suspicious IP addresses, or changing the authentication settings.

It is important to note that only the root user or users with administrative privileges can run the `lastb` command, and that the contents of the `/var/log/btmp` file are usually only accessible to root users. 

## tldr 
 
> Show a listing of last logged in users.
> More information: <https://manned.org/lastb>.

- Show a list of all last logged in users:

`sudo lastb`

- Show a list of all last logged in users since a given time:

`sudo lastb --since {{YYYY-MM-DD}}`

- Show a list of all last logged in users until a given time:

`sudo lastb --until {{YYYY-MM-DD}}`

- Show a list of all logged in users at a specific time:

`sudo lastb --present {{hh:mm}}`

- Show a list of all last logged in users and translate the IP into a hostname:

`sudo lastb --dns`
