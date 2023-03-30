# ac 
## chatgpt 
The 'ac' command is a Linux/Unix command that is used to display the total amount of time spent by a user on a system. 

The output displayed by the 'ac' command typically includes the username of the user whose time is being displayed, the number of hours and minutes the user was logged in, and the date and time of the last system boot.

The 'ac' command is often used by system administrators to keep track of the activities of different users on a system. It can also be used to determine the overall usage patterns of a system and identify potential issues with system performance.

To use the 'ac' command, simply type 'ac' into the terminal and press enter. The output of the command will then be displayed on the screen.

Some common options that can be used with the 'ac' command include '-d' to display the total time spent by users on a particular date, and '-p' to display the time spent by individual users on the system. 

## tldr 
 
> Print statistics on how long users have been connected.
> More information: <https://man.openbsd.org/ac>.

- Print how long the current user has been connected in hours:

`ac`

- Print how long users have been connected in hours:

`ac -p`

- Print how long a particular user has been connected in hours:

`ac -p {{username}}`

- Print how long a particular user has been connected in hours per day (with total):

`ac -dp {{username}}`
