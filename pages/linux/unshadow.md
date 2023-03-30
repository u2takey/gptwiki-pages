# unshadow 
## chatgpt 
The "unshadow" command is a utility that is used to extract password hashes from the /etc/passwd and /etc/shadow files on a Unix or Linux system. These files contain essential information about user accounts, including usernames, user IDs, group IDs, home directories, and encrypted user passwords.

When a user sets up an account on a Unix system, the user's information is stored in the /etc/passwd file. However, for security reasons, the encrypted passwords are stored in the /etc/shadow file. This means that if someone gains unauthorized access to the /etc/passwd file, they still can't easily crack the passwords.

The "unshadow" command is used to combine the /etc/passwd and /etc/shadow files, so that the encrypted passwords can be extracted in one place. This is a useful operation when performing password auditing or testing. Once the encrypted passwords have been extracted, they can be tested against password cracking software or tools like John the Ripper.

To use the "unshadow" command, you would typically run it with the following syntax:

unshadow /etc/passwd /etc/shadow > password-hashes.txt

In this example, the command reads the /etc/passwd and /etc/shadow files and outputs the extracted password hashes to the file "password-hashes.txt". This file can then be used for password auditing or testing. 

## tldr 
 
> Utility provided by the John the Ripper project to obtain the traditional Unix password file if the system uses shadow passwords.
> More information: <https://www.openwall.com/john/>.

- Combine the `/etc/shadow` and `/etc/passwd` of the current system:

`sudo unshadow /etc/passwd /etc/shadow`

- Combine two arbitrary shadow and password files:

`sudo unshadow {{path/to/passwd}} {{path/to/shadow}}`
