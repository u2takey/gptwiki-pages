# pinky 
## chatgpt 
The `pinky` command is a command-line tool used to display information about users on a Unix/Linux system. It provides a way to view the login and logout times of users, as well as their current status and idle time.

When the `pinky` command is executed, it displays the following information for each user:

1. Login name: The name of the user who is currently logged in.
2. TTY: The terminal device associated with the user's session.
3. Remote Host: The name of the remote host (if any) from which the user is logged in.
4. Login Time: The time at which the user logged in.
5. Idle Time: The amount of time the user has been idle since their last activity.
6. JCPU: The accumulated CPU time used by the user's processes.
7. PCPU: The percentage of system CPU time used by the user's processes.
8. Command: The name of the currently running command for the user.

Overall, the `pinky` command can be useful for system administrators to monitor user activity and track logins and logouts. 

## tldr 
 
> Print user information using the `finger` protocol.
> More information: <https://manned.org/pinky>.

- Display details about the current user:

`pinky`

- Display details for a specific user:

`pinky {{user}}`

- Display details in the long format:

`pinky {{user}} -l`

- Omit the user's home directory and shell in long format:

`pinky {{user}} -lb`

- Omit the user's project file in long format:

`pinky {{user}} -lh`

- Omit the column headings in short format:

`pinky {{user}} -f`
