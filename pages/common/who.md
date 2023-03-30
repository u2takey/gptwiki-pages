# who 
## chatgpt 
The "who" command is a Linux/Unix command used to display the information about users who are currently logged in to the system. When this command is run, it will display a list of all users who are currently logged in, their username, the terminal where they are logged in, and the time they logged in.

The basic syntax of the "who" command is as follows:

who [OPTION] [FILE]

Where:

- [OPTION]: represents the optional command-line arguments that can be used with the who command. Some of the commonly used options are -b (displays the time when the system was last booted), -r (displays the current runlevel of the system), -q (displays only the number of users currently logged in instead of displaying their details), etc.

- [FILE]: represents the optional file argument that can be used to obtain the list of users from a specific file instead of the current system.

When the "who" command is run without any options, it will display the list of all users who are currently logged in to the system. This information can be useful in determining who is currently using the system or to monitor user activity on a shared system.

In summary, the "who" command provides information about users who are logged in to the system, including their username, terminal, and login time. It is a useful command for managing user access and monitoring user activity on a Linux/Unix system. 

## tldr 
 
> Display who is logged in and related data (processes, boot time).
> More information: <https://www.gnu.org/software/coreutils/who>.

- Display the username, line, and time of all currently logged-in sessions:

`who`

- Display information only for the current terminal session:

`who am i`

- Display all available information:

`who -a`

- Display all available information with table headers:

`who -a -H`
