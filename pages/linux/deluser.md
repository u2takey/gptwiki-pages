# deluser 
## chatgpt 
The command "deluser" is used to delete a user account in a Unix or Linux operating system. This command is typically used by system administrators to remove old or unused user accounts from the system.

The syntax of the "deluser" command can vary slightly depending on the specific Unix/Linux distribution. However, the basic format is as follows:

deluser [options] username

The options available for the "deluser" command can also vary depending on the distribution, but usually include the ability to remove a user's home directory and mail spool, as well as specifying the removal of any files owned by the user.

For example, to delete a user named "jdoe" from the system, you would enter the following command:

deluser jdoe

If you also want to delete the user's home directory, you can use the "-remove-home" option like this:

deluser --remove-home jdoe

It's important to note that deleting a user account using the "deluser" command is a permanent action and cannot be undone. Therefore, it's advisable to take care when using this command and ensure that you have selected the correct user account to delete. 

## tldr 
 
> Delete a user from the system.
> More information: <https://manpages.debian.org/latest/adduser/deluser.html>.

- Remove a user:

`sudo deluser {{username}}`

- Remove a user and their home directory:

`sudo deluser --remove-home {{username}}`

- Remove a user and their home, but backup their files into a `.tar.gz` file in the specified directory:

`sudo deluser --backup-to {{path/to/backup_directory}} --remove-home {{username}}`

- Remove a user, and all files owned by them:

`sudo deluser --remove-all-files {{username}}`
