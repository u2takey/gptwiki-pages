# setx 
## chatgpt 
The setx command in Windows is used to set a value for specified environment variable in the user or system environment using the command prompt. 

The syntax of the setx command is as follows:

setx variable value [/m]

where
- variable: the name of the environment variable that you want to set the value for.
- value: the value that you want to assign to the environment variable. This can be a string or integer value.
- /m: (optional) used to set the variable in the system environment instead of the user environment.

For example, to set the value of the environment variable "path" with the directory "C:\Windows\System32", you would use the following command:

setx path "C:\Windows\System32" 

This would set the value of the "path" environment variable to "C:\Windows\System32" in the current user environment.

If you want to set the value of the variable in the system environment, you can use the /m option, like this:

setx path "C:\Windows\System32" /m

This command will set the value of the "path" environment variable to "C:\Windows\System32" in the system environment. 

Note that after using the setx command, you will need to close and reopen any command prompt window for the changes to take effect. 

## tldr 
 
> Sets persistent environment variables.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/setx>.

- Set an environment variable for the current user:

`setx {{variable}} {{value}}`

- Set an environment variable for the current machine:

`setx {{variable}} {{value}} /M`

- Set an environment variable for a user on a remote machine:

`setx /s {{hostname}} /u {{username}} /p {{password}} {{variable}} {{value}}`

- Set an environment variable from a registry key value:

`setx {{variable}} /k {{registry\key\path}}`
