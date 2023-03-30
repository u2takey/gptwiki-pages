# systeminfo 
## chatgpt 
The "systeminfo" command is a Windows tool that displays detailed system information about the computer. When the command is entered in the Command Prompt or Run dialog box, it will display the following information:

1. Operating system details - displays the operating system name, version, build number, and other related information.

2. Processor details - shows the processor name, architecture, and speed.

3. Physical memory (RAM) details - displays the installed memory capacity, how much is being used, and how much is available.

4. System type - shows if the operating system is a 32-bit or 64-bit version.

5. BIOS version and date - shows the BIOS manufacturer, version, and install date.

6. Computers manufacturer and model - shows the manufacturer and model of the computer.

7. Network adapter details - displays the details of all installed network adapters and their respective IP addresses.

8. Time zone and local time - shows the time zone and local time of the computer.

Overall, "systeminfo" is a useful command for obtaining information about your computer's hardware and software configuration. It is frequently used by system administrators and IT professionals to diagnose and troubleshoot computer issues. 

## tldr 
 
> Display operating system configuration for a local or remote machine.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/systeminfo>.

- Display system configuration for the local machine:

`systeminfo`

- Display system configuration in a specified output format:

`systeminfo /fo {{table|list|csv}}`

- Display system configuration for a remote machine:

`systeminfo /s {{remote_name}} /u {{username}} /p {{password}}`

- Display detailed usage information:

`systeminfo /?`
