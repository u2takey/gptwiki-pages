# set 
## chatgpt 
"set" is a command used in various operating systems, including Linux, macOS, and Windows, to manipulate various environment variables or shell attributes. 

In Linux and macOS, the "set" command without any arguments is used to display all environment variables currently set in the shell session. These can include system-level variables like the PATH variable, which tells the shell where to look for executable files when a command is entered, or user-level variables that have been defined by the user running the shell.

The "set" command can also be used to set or modify environment variables in the shell session. For example, to set a variable called "MY_VARIABLE" to the value "hello world", the command "set MY_VARIABLE=hello world" can be used. This will create a new environment variable called MY_VARIABLE that can be accessed in subsequent commands or scripts.

In Windows, the "set" command can be used to set or display environment variables as well. However, the syntax for setting variables in Windows differs from Linux and macOS. In Windows, the command to set a variable is "set VAR_NAME=VALUE", without any spaces before or after the equals sign. 

Overall, the "set" command is a versatile tool that can be used to manage environment variables and shell settings across different operating systems. 

## tldr 
 
> Display, set or unset values of shell attributes and positional parameters.
> More information: <https://manned.org/set>.

- Display the names and values of shell variables:

`set`

- Mark variables that are modified or created for export:

`set -a`

- Notify of job termination immediately:

`set -b`

- Set various options, e.g. enable `vi` style line editing:

`set -o {{vi}}`

- Set the shell to exit as soon as the first error is encountered (mostly used in scripts):

`set -e`
