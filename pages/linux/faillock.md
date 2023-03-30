# faillock 
## chatgpt 
The "faillock" command is a tool used in Linux operating systems to manage login failures for user accounts. It allows system administrators to track and control the number of unsuccessful login attempts a user can make before their account is locked. 

Syntax: 

The basic syntax of the "faillock" command is as follows:

```
faillock [options] username
```

Options: 

The "faillock" command provides a variety of options that can be used in conjunction with the command to customize its functionality. Some of these options include:

- "-m", "--max-attempts": Sets the maximum number of login attempts a user can make before their account is locked. 
- "-u", "--unlock": Unlocks a locked user account. 
- "-r", "--reset": Resets the count of failed login attempts for a user. 
- "-t", "--interval": Sets the duration of time in seconds that a user must wait after a failed login attempt before they can try again. 
- "-h", "--help": Displays help information for the command.

Example:

To lock an account after three failed login attempts:

```
faillock --max-attempts 3 john
```

To unlock a locked account:

```
faillock --unlock john
```

To reset the count of failed login attempts for a user:

```
faillock --reset john
```

To set the time interval between failed login attempts:

```
faillock --interval 60 john
```

In summary, the "faillock" command is a useful tool for system administrators to manage login failures and ensure the security of user accounts on Linux systems. It allows administrators to set limits on login attempts, unlock locked accounts, and reset failed login attempts for users. 

## tldr 
 
> Display and modify authentication failure record files.
> More information: <https://manned.org/faillock>.

- List login failures of all users:

`sudo faillock`

- List login failures of the specified user:

`sudo faillock --user {{user}}`

- Reset the failure records of the specified user:

`sudo faillock --user {{user}} --reset`
