# tzutil 
## chatgpt 
tzutil is a command-line utility in Windows operating systems that allows users to manage and change time zones. Here are the details of commonly used tzutil commands:

1. tzutil /g: This command shows the current time zone of your system.

2. tzutil /l: This command lists all the available time zones that you can set on your system.

3. tzutil /s: This command sets the time zone for your system. You just need to specify the time zone you want to set with the command.

4. tzutil /? : This command gives detailed help about how the tzutil command works and the parameters that can be used with it.

Overall, tzutil command provides a convenient way for the users to manage time zones on their Windows systems, making it easier to keep up with time changes and avoid confusion when collaborating with others across different time zones. 

## tldr 
 
> A tool for displaying or configuring the system time zone.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/tzutil>.

- Get the current time zone:

`tzutil /g`

- Display a list of available time zones:

`tzutil /l`

- Set the system time zone to the specific value:

`tzutil /s {{timezone_id}}`
