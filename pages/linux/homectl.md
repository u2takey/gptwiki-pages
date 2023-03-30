# homectl 
## chatgpt 
The "homectl" command is used in Linux-based operating systems to manage user home directories. This command allows the system administrator to create, delete, and modify user accounts along with their respective home directories.

The following are some of the commonly used options with the homectl command:

- homectl create [USERNAME]: This command is used to create a new user account with their home directory. The home directory will be created under the directory specified in the "Home" field of the /etc/default/useradd file.

- homectl delete [USERNAME]: This command is used to delete a user account including their home directory.

- homectl lock [USERNAME]: This command is used to lock a user account so that they cannot log in.

- homectl unlock [USERNAME]: This command is used to unlock a previously locked user account.

- homectl update [USERNAME] --shell [SHELL]: This command is used to update the user's shell to the specified shell.

Overall, homectl is a useful command for managing user accounts and their home directories on Linux-based operating systems. 

## tldr 
 
> Create, remove, change or inspect home directories using the systemd-homed service.
> More information: <https://manned.org/homectl>.

- List user accounts and their associated home directories:

`homectl list`

- Create a user account and their associated home directory:

`sudo homectl create {{username}}`

- Remove a specific user and the associated home directory:

`sudo homectl remove {{username}}`

- Change the password for a specific user:

`sudo homectl passwd {{username}}`

- Run a shell or a command with access to a specific home directory:

`sudo homectl with {{username}} -- {{command}} {{command_arguments}}`

- Lock or unlock a specific home directory:

`sudo homectl {{lock|unlock}} {{username}}`

- Change the disk space assigned to a specific home directory to 100 GiB:

`sudo homectl resize {{username}} {{100G}}`

- Display help:

`homectl --help`
