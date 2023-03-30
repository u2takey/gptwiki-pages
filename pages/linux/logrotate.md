# logrotate 
## chatgpt 
Logrotate is a command-line utility used in Unix-based operating systems to manage and rotate log files. 

When applications or system services generate log files, they can take up a significant amount of disk space if the log files are not managed properly. Logrotate provides an automated way to rotate, compress, and delete old log files on a scheduled basis.

The logrotate command takes a configuration file that specifies the location of the log files, how often they should be rotated, and how many old log files to keep. The configuration file can also specify options for compressing, copying, or emailing the rotated logs.

Logrotate is typically run as a scheduled task using the cron daemon or systemd timers on Linux. The frequency of rotation depends on the requirements of the application and the amount of disk space available.

Overall, logrotate is an essential tool for managing log files and preventing disk space issues. It ensures that logs are efficiently rotated, archived, and deleted, keeping the system running smoothly. 

## tldr 
 
> Rotates, compresses, and mails system logs.
> More information: <https://manned.org/logrotate>.

- Trigger a run manually:

`logrotate {{path/to/logrotate.conf}} --force`

- Run using a specific command to mail reports:

`logrotate {{path/to/logrotate.conf}} --mail {{/usr/bin/mail_command}}`

- Run without using a state (lock) file:

`logrotate {{path/to/logrotate.conf}} --state /dev/null`

- Run and skip the state (lock) file check:

`logrotate {{path/to/logrotate.conf}} --skip-state-lock`

- Tell `logrotate` to log verbose output into the log file:

`logrotate {{path/to/logrotate.conf}} --log {{path/to/log_file}}`
