# leave 
## chatgpt 
The "leave" command is a terminal command used to set a time limit on a shell session. It is often used when a user is working remotely or on a shared system and wants to ensure that they do not keep a shell session open for too long.

When the "leave" command is executed, the user is prompted to enter the time duration for the shell session. The duration can be entered in several different formats, including minutes or hours.

Once the duration is set, the user can continue to work in the shell session as normal. However, after the specified time duration expires, the shell session will automatically terminate and the user will be logged out.

The "leave" command is a useful tool for managing system resources and ensuring that shell sessions do not consume excessive computing power. It can help prevent security risks, improve system performance, and promote responsible use of shared computing resources. 

## tldr 
 
> Set a reminder for when it's time to leave.
> To remove reminders use `kill $(pidof leave)`.
> More information: <https://www.freebsd.org/cgi/man.cgi?query=leave>.

- Set a reminder at a given time:

`leave {{time_to_leave}}`

- Set a reminder to leave at noon:

`leave {{1200}}`

- Set a reminder in a specific amount of time:

`leave +{{amount_of_time}}`

- Set a reminder to leave in 4 hours and 4 minutes:

`leave +{{0404}}`
