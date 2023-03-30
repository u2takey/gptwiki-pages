# newgrp 
## chatgpt 
The "newgrp" command is a Linux command that allows the user to change their current group ID to another group ID. This command is useful in situations where the user needs to work with a different set of privileges or permissions, which are assigned to a specific group. This command is also used to create a new shell process with the specified group ID.

The syntax of the newgrp command is as follows:

newgrp [group name]

Here, the group name is the name of the group to which the user wants to switch.

When the newgrp command is executed, it checks if the user is a member of the specified group. If the user is not a member of the group, it displays an error message and does not change the group ID.

If the user is a member of the group, newgrp changes the group ID of the user and creates a new shell process for the user with the specified group ID. This new shell process inherits all the environment variables and settings of the original shell process, but it has the privileges and permissions of the specified group.

The newgrp command is often used in combination with the "groups" command, which shows the groups that the user is a member of. By running "groups" before and after using the newgrp command, the user can verify that the group ID has indeed been changed. 

## tldr 
 
> Switch primary group membership.
> More information: <https://manned.org/newgrp>.

- Change user's primary group membership:

`newgrp {{group_name}}`

- Reset primary group membership to user's default group in `/etc/passwd`:

`newgrp`
