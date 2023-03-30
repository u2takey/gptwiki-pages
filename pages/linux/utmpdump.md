# utmpdump 
## chatgpt 
The "utmpdump" command is a utility program that allows you to examine the contents of the UTMP and WTMP files on Unix and Unix-like operating systems. UTMP stands for "user accounting database" and WTMP stands for "system accounting database". These files are used to record information about user login sessions, system boot and shutdown times, and other related events.

The "utmpdump" command reads the UTMP and/or WTMP files and prints the contents in a human-readable format. This can be useful for troubleshooting login or other system-related issues, tracking system usage, or auditing user activity.

Some examples of how the "utmpdump" command can be used are:

- To display the contents of the UTMP file:

  `utmpdump /var/run/utmp`

- To display the contents of the WTMP file:

  `utmpdump /var/log/wtmp`

- To display the contents of both the UTMP and WTMP files:

  `utmpdump /var/run/utmp /var/log/wtmp`

- To display the contents of the WTMP file in reverse order (i.e. most recent events first):

  `utmpdump -r /var/log/wtmp`

The output of the "utmpdump" command will typically include information such as:

- The type of event (e.g. login, logout, boot, shutdown)
- The date and time of the event
- The user account name
- The terminal device or IP address used for the session
- Other relevant details such as the system hostname or process ID

Overall, the "utmpdump" command is a helpful tool for system administrators and users who need to examine or analyze the system accounting data recorded in the UTMP and WTMP files. 

## tldr 
 
> Dump and load btmp, utmp and wtmp accounting files.
> More information: <https://manned.org/utmpdump>.

- Dump the `/var/log/wtmp` file to the standard output as plain text:

`utmpdump {{/var/log/wtmp}}`

- Load a previously dumped file into `/var/log/wtmp`:

`utmpdump -r {{dumpfile}} > {{/var/log/wtmp}}`
