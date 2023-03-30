# reg add 
## chatgpt 
"Reg add" is a command used in Windows operating systems to add a new value, key or subkey to the Registry. The Registry is a database that stores configuration settings, software and hardware settings, user preferences and other critical system data for Windows. 

Following are the parameters used with the "reg add" command:

1. Key: This parameter specifies the location in the Registry where the new value, key or subkey will be added.

2. /v: This parameter specifies the name of the value that will be added.

3. /t: This parameter specifies the type of the value that will be added. The following data types are supported: REG_SZ, REG_MULTI_SZ, REG_DWORD, REG_QWORD, REG_BINARY, and REG_EXPAND_SZ.

4. /d: This parameter specifies the data for the value. It varies according to the data type specified with the /t parameter.

5. /f: This parameter forces the operation without prompting for confirmation.

For example, the following command adds a new key named "MyKey" under the "HKEY_CURRENT_USER\Software" key:

reg add HKCU\Software\MyKey

The following command adds a new string value named "MyValue" with data "test" under the "MyKey" key:

reg add HKCU\Software\MyKey /v MyValue /t REG_SZ /d test

Overall, "reg add" is a powerful command that can be used by advanced users and system administrators to manage Windows Registry settings. It should be used with caution and a good understanding of the consequences of the changes made. 

## tldr 
 
> Add new keys and their values to the registry.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/reg-add>.

- Add a new registry key:

`reg add {{key_name}}`

- Add a new value under a specific key:

`reg add {{key_name}} /v {{value}}`

- Add a new value with specific data:

`reg add {{key_name}} /d {{data}}`

- Add a new value to a key with a specific data type:

`reg add {{key_name}} /t {{type}}`

- Forcefully overwrite the existing registry value without a prompt:

`reg add {{key_name}} /f`
