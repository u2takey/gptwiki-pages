# lastlog 
## chatgpt 
The lastlog command displays the recent login history for all the users on the system. When executed without any options, this command will display a list of all users who have ever logged into the system and when their last login occurred. The output includes the user's account name, their last login time and date, as well as their IP address if they logged in remotely. 

If the -b or --before option is used, it allows to see the list of users who have not logged in since a specified time. The time can be specified in various formats like months, weeks, days, hours, minutes or a specific date, after which the login attempts of the users who have not logged in since then will be displayed.

Similarly, the -t or --time option allows to see the list of users who have logged in since a specified time. The time can be specified in the same format as for the -b option, and the command will display the login attempts of the users who have logged in since then.

Overall, the lastlog command is a helpful tool for system administrators to keep track of the user login activity and how often different user accounts are being used. 

## tldr 
 
> Show the most recent login of all users or of a given user.
> More information: <https://manned.org/lastlog>.

- Display the most recent login of all users:

`lastlog`

- Display the lastlog record of the specified user:

`lastlog --user {{username}}`

- Display records older than 7 days:

`lastlog --before {{7}}`

- Display records more recent than 3 days:

`lastlog -time {{3}}`
