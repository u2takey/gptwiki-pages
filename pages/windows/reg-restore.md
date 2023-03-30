# reg restore 
## chatgpt 
The "reg restore" command is a Windows command used to restore the contents of a registry hive from a backup file. 

Here's how it works:

1. Open the Command Prompt or PowerShell app as an administrator by searching for "cmd" or "PowerShell" in the Start menu, right-clicking on it, and selecting "Run as administrator."

2. Type "reg restore" followed by the key path and filename of the backup file you want to restore, and then press Enter. For example, if your backup file is named "hklm_backup.reg" and is located in the "C:\Users\Username\Documents" folder, you would type the following command:

reg restore HKLM\C:\Users\Username\Documents\hklm_backup.reg

3. If the backup file contains any data that already exists in the registry, you will be prompted to either overwrite the data, append it to the existing data, or not restore the conflicting data. Make your selection and press Enter.

4. If the restoration was successful, you will see a message indicating that the operation was completed successfully.

Using the "reg restore" command allows you to restore your registry settings to a previous state, which can be useful if you encounter errors or other issues with your current settings. Note that restoring the registry from a backup file will overwrite any changes made to the registry since the backup was created, so use this command with caution. 

## tldr 
 
> Restore a key and its values from a backup file.
> See `reg-save` for more information.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/reg-restore>.

- Overwrite a specified key with data from a backup file:

`reg restore {{key_name}} {{path\to\file}}`
