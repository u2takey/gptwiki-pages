# date 
## chatgpt 
The "date" command is a command-line utility in Unix-based operating systems that displays the system date and time. When this command is entered in the terminal, the current date and time in the local time zone are displayed.

By default, the "date" command will display the date and time in a standardized format that includes the day of the week, month, day, time, time zone, and year. The format of the output can be customized using various format options with the command.

Some of the most common options used with the "date" command include:

- "+FORMAT": This option allows you to customize the format of the date and time output. For example, to display only the time, you can use the command "date +%T".

- "-s STRING": This option allows you to set the system date and time to a specific value. For example, to set the system time to 4:30 PM on March 15, 2022, you can use the command "date -s '2022-03-15 16:30:00'".

- "-u": This option displays the date and time in UTC (Coordinated Universal Time) rather than in the local time zone.

Overall, the "date" command is a useful tool for displaying and manipulating the date and time on Unix-based systems. 

## tldr 
 
> Displays or sets the system date.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/date>.

- Display the current system date and prompt to enter a new date (leave empty to keep unchanged):

`date`

- Display the current system date without prompting for a new date:

`date /t`

- Change the current system date to a specific date:

`date {{month}}-{{day}}-{{year}}`
