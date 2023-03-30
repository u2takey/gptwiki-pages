# adduser 
## chatgpt 
The `adduser` command is used in Unix-based operating systems like Linux and macOS to create a new user account on the system.

The syntax for the `adduser` command is:

```
adduser [username]
```

Where `[username]` is the name of the user account you want to create. When you run the `adduser` command, the system prompts you to enter additional information about the user, including:

- Full name: This can be the user's actual name, or any other identifier you choose.
- Room/Building: This field is usually used to identify the physical location of the user.
- Work Phone: The phone number the user can be reached at during work hours.
- Home Phone: The user's phone number at home.
- Other: Any additional information you want to add about the user.

Once you have entered this information, the system creates a new user account with a home directory and a default set of permissions. The user can then log in and begin using the system. 

The `adduser` command has several optional flags that can be used to customize the user account creation process. For example, you can use the `-s` flag to specify a different default shell for the user, or the `-m` flag to create the user's home directory if it doesn't already exist. 

It's worth noting that the `adduser` command can only be run by a system administrator or a user with sudo privileges. This is because creating new user accounts can have significant security implications and could potentially compromise the entire system. 

## tldr 
 
> User addition utility.
> More information: <https://manpages.debian.org/latest/adduser/adduser.html>.

- Create a new user with a default home directory and prompt the user to set a password:

`adduser {{username}}`

- Create a new user without a home directory:

`adduser --no-create-home {{username}}`

- Create a new user with a home directory at the specified path:

`adduser --home {{path/to/home}} {{username}}`

- Create a new user with the specified shell set as the login shell:

`adduser --shell {{path/to/shell}} {{username}}`

- Create a new user belonging to the specified group:

`adduser --ingroup {{group}} {{username}}`
