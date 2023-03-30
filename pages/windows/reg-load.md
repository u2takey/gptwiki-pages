# reg load 
## chatgpt 
"Reg load" is a command in Windows operating system that is used to load a hive file into the registry. The registry is a central database in Windows that stores configuration settings and options for the operating system and installed programs. A hive file is a part of the registry that contains a set of keys, subkeys, and their associated values.

To use the "reg load" command, you need to have administrative privileges. The syntax of the command is as follows:

reg load HKLM\Key_Name File_Path

Here, "HKLM" refers to the "HKEY_LOCAL_MACHINE" hive in the registry, which contains system-wide settings and preferences. "Key_Name" is the name for the hive file that you want to load, and "File_Path" is the full path to the hive file on your computer.

When you run the command, Windows loads the contents of the specified hive file into the registry under the specified key. You can then use various registry editing tools to modify or view the settings in the loaded hive.

For example, if you have a backup of the System hive file (system.dat) from a previous installation of Windows, you can use the "reg load" command to load it into the registry and examine its contents. You could then extract important settings or data that might be useful for troubleshooting or system recovery purposes. 

## tldr 
 
> Load saved sub keys into a different sub key in the registry.
> This is intended for troubleshooting and temporary keys.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/reg-load>.

- Load a backup file into the specified key:

`reg load {{key_name}} {{path\to\file}}`
