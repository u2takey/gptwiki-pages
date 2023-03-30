# reg copy 
## chatgpt 
The "reg copy" command is a Windows command used to copy registry keys and their values from one location to another. It is used to backup or restore registry settings, transfer settings from one computer to another or to implement changes to multiple computers.

The "reg copy" command is a command line tool that uses the following syntax: 

reg copy [source registry key] [destination registry key] [/s]

Source Registry Key: Specifies the registry key that you want to copy from. It can be specified as a complete path or hive abbreviation. For example, HKEY_CURRENT_USER\Control Panel\Desktop or HKCU\Control Panel\Desktop.

Destination Registry Key: Specifies the path to the new location. It can be specified as a complete path or hive abbreviation.

/S (Optional): Copies the registry subkeys and values recursively.

Once you execute the command, it will copy the specified key and its values from the source to the destination location.

Note that the "reg copy" command requires administrative privileges to execute and should be used with caution as modifying the registry incorrectly can cause system instability or even render the system unusable. 

## tldr 
 
> Copy keys and their values in the registry.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/reg-copy>.

- Copy a registry key to a new registry location:

`reg copy {{old_key_name}} {{new_key_name}}`

- Copy a registry key recursively to a new registry location:

`reg copy {{old_key_name}} {{new_key_name}} /s`

- Forcefully copy a registry key without a prompt:

`reg copy {{old_key_name}} {{new_key_name}} /f`
