# date 
## chatgpt 
The 'date' command is a command that displays the current date and time on a Linux or Unix-based system. It can be used in the terminal of the operating system to display the current date, and/or to set the date and time to a specified value.

When you run the 'date' command without any arguments, it will simply display the current date and time in the default format determined by the operating system. For example, it can display a date and time like this : "Thu Oct 7 21:15:52 UTC 2021".

The 'date' command can also be used with various options and arguments to format the output of the date and time according to specific requirements. For example, 'date +%Y-%m-%d' will display the date in the format 'yyyy-mm-dd', while 'date +%H:%M:%S' will display the time as 'hh:mm:ss'.

Besides displaying the date and time, the 'date' command can also be used to change the system time. However, changing the system time requires root or administrator privileges. The syntax for changing the date and time is like this: 'date -s "MM/DD/YYYY HH:MM:SS"'. This means you can set the time and date with required values in the format "Month/Day/Year Hour:Minute:Second". However, providing the correct format for setting the date and time is important. 

## tldr 
 
> Set or display the system date.
> More information: <https://www.gnu.org/software/coreutils/date>.

- Display the current date using the default locale's format:

`date +%c`

- Display the current date in UTC, using the ISO 8601 format:

`date -u +%Y-%m-%dT%H:%M:%S%Z`

- Display the current date as a Unix timestamp (seconds since the Unix epoch):

`date +%s`

- Convert a date specified as a Unix timestamp to the default format:

`date -d @{{1473305798}}`

- Convert a given date to the Unix timestamp format:

`date -d "{{2018-09-01 00:00}}" +%s --utc`

- Display the current date using the RFC-3339 format (`YYYY-MM-DD hh:mm:ss TZ`):

`date --rfc-3339=s`

- Set the current date using the format `MMDDhhmmYYYY.ss` (`YYYY` and `.ss` are optional):

`date {{093023592021.59}}`

- Display the current ISO week number:

`date +%V`
