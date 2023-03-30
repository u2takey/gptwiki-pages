# reg query 
## chatgpt 
The "reg query" command is a command-line utility that allows the user to query the Windows registry for various information. 

The "reg" part of the command is short for "registry," which is a hierarchical database that stores settings and configuration information for Microsoft Windows operating systems.

The "query" part of the command specifies that the user wants to perform a query of the registry, which can be used to retrieve information about a particular registry key or value.

The specific syntax of the "reg query" command will depend on the type of information the user wants to retrieve from the registry. For example, a simple "reg query" command might look like this:

reg query HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows

This command retrieves information about the Windows registry keys stored under the HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows path.

Overall, the "reg query" command is a powerful tool that can be used to retrieve valuable information about a Windows computer's configuration and settings. However, it should be used with caution, as modifying the registry can have serious consequences if done improperly. 

## tldr 
 
> Display the values of keys and sub keys in the registry.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/reg-query>.

- Display all values of a key:

`reg query {{key_name}}`

- Display a specific value of a key:

`reg query {{key_name}} /v {{value}}`

- Display all values of a key and its sub keys:

`reg query {{key_name}} /s`

- Search for keys and values matching a specific pattern:

`reg query {{key_name}} /f "{{query_pattern}}"`

- Display a value of a key matching a specified data type:

`reg query {{key_name}} /t {{type}}`
