# usermod 
## chatgpt 
The usermod command is a Linux command that is used to modify an existing user account. The command allows the user to change various attributes of the user account including the user's name, password, home directory, login shell, and group membership.

The syntax for the command is:

usermod [options] username

Here, 'options' are the various options that can be used along with the command to modify the user account.

Some commonly used options with the usermod command are:

- -c: This option is used to add a comment to the user's account. The comment can be anything that describes the user or their role.

- -d: This option is used to change the user's home directory. By default, the home directory is set to /home/username.

- -g: This option is used to change the user's primary group. By default, the primary group is set to the same name as the username.

- -s: This option is used to change the user's login shell. By default, the login shell is set to /bin/bash.

- -L: This option is used to lock the user's account. Once the account is locked, the user will not be able to log in.

- -U: This option is used to unlock the user's account if it has been locked using the -L option.

Example:

To change the primary group of a user to 'developers', we can use the following command:

usermod -g developers username

This will change the primary group of the user 'username' to 'developers'. 

## tldr 
 
> Modifies a user account.
> See also: `users`, `useradd`, `userdel`.
> More information: <https://manned.org/usermod>.

- Change a username:

`sudo usermod --login {{new_username}} {{username}}`

- Change a user id:

`sudo usermod --uid {{id}} {{username}}`

- Change a user shell:

`sudo usermod --shell {{path/to/shell}} {{username}}`

- Add a user to supplementary groups (mind the lack of whitespace):

`sudo usermod --append --groups {{group1,group2,...}} {{username}}`

- Change a user home directory:

`sudo usermod --move-home --home {{path/to/new_home}} {{username}}`
