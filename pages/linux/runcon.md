# runcon 
## chatgpt 
The "runcon" command is a Linux command that is used to run a command with a specified security context. The security context includes information such as the SELinux context or user ID that the command should run as.

The syntax for the command is as follows:

```
runcon [-u user] [-r role] [-t type] command [args...]
```

- The "-u" option specifies the user ID to run the command as.
- The "-r" option specifies the SELinux role to run the command as.
- The "-t" option specifies the SELinux type to run the command as.
- The "command" is the actual command to be executed, along with any arguments.

For example, if you want to run the "ls" command with a modified security context, you could use:

```
runcon -t my_selinux_type ls -l
```

This will run the "ls" command with the SELinux type "my_selinux_type". 

The "runcon" command is commonly used in SELinux environments to ensure that commands are executed with the appropriate security context, which can help prevent unauthorized access to files and resources. 

## tldr 
 
> Run a program in a different SELinux security context.
> With neither context nor command, print the current security context.
> More information: <https://www.gnu.org/software/coreutils/runcon>.

- Determine the current domain:

`runcon`

- Specify the domain to run a command in:

`runcon -t {{domain}}_t {{command}}`

- Specify the context role to run a command with:

`runcon -r {{role}}_r {{command}}`

- Specify the full context to run a command with:

`runcon {{user}}_u:{{role}}_r:{{domain}}_t {{command}}`
