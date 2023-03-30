# last 
## chatgpt 
The command "last" is used in Linux and Unix operating systems to display a list of users who have recently logged in and out of the system. The output of the command provides information about the user's login name, the terminal used to connect and the time of the login or logout.

The command can be used with several options to filter the output. Some of the commonly used options include:

- -a: This option displays information about all logins and logouts, including system reboots.
- -d: This option displays only the date (rather than time) of the last login for each user.
- -F: This option displays the full login and logout times, including date, month, day, time, and year.
- -i: This option displays the IP address of the remote host from which the user logged in.
- -n: This option displays the number of recent logins specified by the user.
- -t: This option displays the last time the system was booted.

Example Usage:

To display the last 10 logins, use the following command:

$ last -n 10

To display the last 10 reboots, use the following command:

$ last -a -n 10 -F | grep reboot

To display the last login time for a specific user, use the following command:

$ last | grep username 

## tldr 
 
> View the last logged in users.
> More information: <https://manned.org/last>.

- View last logins, their duration and other information as read from `/var/log/wtmp`:

`last`

- Specify how many of the last logins to show:

`last -n {{login_count}}`

- Print the full date and time for entries and then display the hostname column last to prevent truncation:

`last -F -a`

- View all logins by a specific user and show the IP address instead of the hostname:

`last {{username}} -i`

- View all recorded reboots (i.e., the last logins of the pseudo user "reboot"):

`last reboot`

- View all recorded shutdowns (i.e., the last logins of the pseudo user "shutdown"):

`last shutdown`
