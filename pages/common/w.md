# w 
## chatgpt 
The `w` command is a Linux/Unix command used to display information about the users who are currently logged in and their activity. When the `w` command is executed, it displays the following information for each user:

- User's name
- Terminal or TTY (Teletype) device used for the login
- Remote host from where the user has logged in
- Login time
- Idle time (time since the user has last interacted with the terminal)
- JCPU (Jiffy CPU) time used by all processes attached to the user's tty
- PCPU (Process CPU) time used by the user's process
- Command line of the current process

Example output of the `w` command:
```
 19:47:12 up 1 day,  8:13,  1 user,  load average: 0.02, 0.01, 0.00
USER     TTY      FROM             LOGIN@   IDLE   JCPU   PCPU WHAT
user     tty1     -                Thu16    1:48m  0.16s  0.11s -bash
```

In the example output above, the `w` command displays the current system time, uptime, number of users logged in, and the system load average. For the only user logged in (`user`), it displays information on the TTY device used, the remote login location, login time, idle time, and CPU usage statistics. It also displays the current process running for the user. 

## tldr 
 
> Show who is logged on and what they are doing.
> Print user login, TTY, remote host, login time, idle time, current process.
> More information: <https://manned.org/w>.

- Show logged-in users info:

`w`

- Show logged-in users info without a header:

`w -h`
