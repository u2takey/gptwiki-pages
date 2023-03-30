# reg flags 
## chatgpt 
The "reg flags" command is not a specific or recognized command in most operating systems or command line interfaces. "Reg" could potentially be short for "registry," which is a database used by Windows operating systems to store configuration information. However, without context or more information, it is impossible to provide a detailed explanation of the command. 

## tldr 
 
> Display or set flags on registry keys.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/reg-flags>.

- Display current flags for a specific key:

`reg flags {{key_name}} query`

- Display help and available flag types:

`reg flags /?`

- Set specified space-separated flags, and unset unmentioned flags, for a specific key:

`reg flags {{key_name}} set {{flag_names}}`

- Set specified flags for a specific key and its sub keys:

`reg flags {{key_name}} set {{flag_names}} /s`
