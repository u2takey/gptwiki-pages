# vipw 
## chatgpt 
The command "vipw" opens up the /etc/passwd file for editing. This file contains the usernames, passwords, user IDs, home directories, and default shells for all the users on the system. The command is meant to be run by the system administrator to change the user account information or to add new users to the system.

Once the command is executed, the system opens up the /etc/passwd file in the default text editor specified in the system's environment variables. It is important to note that the file should only be modified by the system administrator and that changes made to the file can have a significant impact on the system's security.

After the changes are made, the system administrator can save and exit the file, and the changes take effect immediately. 

## tldr 
 
> Edit the password file.
> More information: <https://manned.org/vipw>.

- Edit the password file:

`vipw`

- Display the current version of `vipw`:

`vipw --version`
