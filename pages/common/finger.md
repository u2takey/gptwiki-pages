# finger 
## chatgpt 
The "finger" command is a command-line tool used in Unix/Linux systems to display information about a specific user on the system. When you execute the "finger" command followed by a username, it displays information like their login name, real name, user ID, login time, terminal, and other details about the user.

The finger command can also display information about user's home directory, email address, and the last time they logged in.

Here is the syntax for the "finger" command:

finger [options] [username]

The options that can be used with the finger command are:

- -l: Displays a long-format listing that includes the user's home directory, shell, and last login time.
- -m: Sends output in mail format.
- -s: Changes the source of the information to be displayed.

For example, to check the information about a user "john", you can use the following command:

finger john

This will display the following information about John:

- Login name
- Real name
- Directory
- Shell
- Last login
- Idle time
- JCPU
- PCPU
- Time since last login
- Login terminal

Overall, the finger command is a simple and useful tool to check the status and details of the user accounts on a Unix/Linux system. 

## tldr 
 
> User information lookup program.
> More information: <https://manned.org/finger>.

- Display information about currently logged in users:

`finger`

- Display information about a specific user:

`finger {{username}}`

- Display the user's login name, real name, terminal name, and other information:

`finger -s`

- Produce multiline output format displaying same information as `-s` as well as user's home directory, home phone number, login shell, mail status, etc.:

`finger -l`

- Prevent matching against user's names and only use login names:

`finger -m`
