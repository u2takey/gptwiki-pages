# chage 
## chatgpt 
The "chage" command in Linux is used to change the password expiration and other aging information. It is used to manage the user password expiry information on Linux systems. 

The chage command can be used to perform any of the following tasks:
- Set password expiration date
- Set password minimum and maximum age
- Set password warning period
- Disable password aging

Syntax: 

    chage [options] USERNAME

Options:
- -d, --lastday: This option sets the date on which the password was last changed to yyyy-mm-dd.
- -E, --expiredate: This option sets the date on which the user account will be disabled.
- -I, --inactive: This option sets the number of days of inactivity (after password expiration) after which the user account will be disabled.
- -m, --mindays: This option sets the minimum number of days required between password changes.
- -M, --maxdays: This option sets the maximum number of days during which a password is valid.
- -W, --warndays: This option sends a warning message to the user that their password will expire in X days.

Example:

To set the password expiry date of a user "testuser" to June 7th, 2022, the command would be:

    chage -E 2022-06-07 testuser

This will set the expiry date of the user "testuser" to June 7th, 2022.

To set the maximum number of days during which a password is valid to 90 days for the user "testuser", the command would be:

    chage -M 90 testuser

This will set the maximum password age for the user "testuser" to 90 days. 

In summary, the chage command is a useful Linux command that can be used to manage the password expiry and aging information for user accounts. 

## tldr 
 
> Change user account and password expiry information.
> More information: <https://manned.org/chage>.

- List password information for the user:

`chage --list {{username}}`

- Enable password expiration in 10 days:

`sudo chage --maxdays {{10}} {{username}}`

- Disable password expiration:

`sudo chage --maxdays {{-1}} {{username}}`

- Set account expiration date:

`sudo chage --expiredate {{YYYY-MM-DD}} {{username}}`

- Force user to change password on next log in:

`sudo chage --lastday {{0}} {{username}}`
