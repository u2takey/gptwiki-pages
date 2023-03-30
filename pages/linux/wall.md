# wall 
## chatgpt 
The "wall" command is a Unix/Linux command that is used to send a message to all users that are currently logged in on the system. The message is displayed in the terminal window of each user, blocking any activity until the message is acknowledged.

Syntax:
wall [message]

The "message" argument is optional, and if not provided, the command will wait for input from standard input.

Example:
To send a simple message to all users, type the following command:

wall "Hello everyone, we will be having a scheduled maintenance at 6 PM today. Please save your work and log out."

This will send the message to all users currently logged in on the system.

Once the message is sent, all users will see the message displayed in their terminal window. They can then acknowledge the message by typing any key. Once every user has acknowledged the message, they can resume their work. 

## tldr 
 
> Write a message on the terminals of users currently logged in.
> More information: <https://manned.org/wall>.

- Send a message:

`wall {{message}}`

- Send a message to users that belong to a specific group:

`wall --group {{group_name}} {{message}}`

- Send a message from a file:

`wall {{file}}`

- Send a message with timeout (default 300):

`wall --timeout {{seconds}} {{file}}`
