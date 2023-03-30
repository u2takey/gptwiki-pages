# finger 
## chatgpt 
The `finger` command is a command-line tool in Unix-like operating systems that is used to display information about a user or users on a system. The command is named `finger` because it was originally designed to provide a quick and easy way to find out who was "pointing the finger" at a particular machine.

When the `finger` command is entered, followed by the username (s) you want to display information for, the output will include the full name, login name, terminal name, idle time, login time, and any plan the user has written. This information is sourced from the `passwd` file and the `utmp` database (or its modern replacement, `wtmp`).

For example, if you want to display information about the user `jdoe`, you would enter:

```
finger jdoe
```

The output will look something like this:

```
Login:        jdoe                        Name: John Doe
Directory:    /home/jdoe                  Shell: /bin/bash
Office:                                      Office Phone: 
On since Thu Jun 17 11:05 (EDT) on tty1      1 hour 30 minutes idle
Last login Thu Jun 17 11:05 (EDT) on tty1
Mail last read Tue May 11 10:10 (EDT) on tty3
Plan:         Working on a new project
```

Overall, the `finger` command is a simple and useful tool for quickly getting details about users on a Unix-like system. 

## tldr 
 
> Return information about one or more users on a specified system.
> The remote system must be running the Finger service.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/finger>.

- Display information about a specific user:

`finger {{user}}@{{host}}`

- Display information about all users on the specified host:

`finger @{{host}}`

- Display information in a longer format:

`finger {{user}}@{{host}} -l`

- Display help information:

`finger /?`
