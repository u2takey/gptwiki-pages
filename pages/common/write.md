# write 
## chatgpt 
The "write" command is used to write messages or lines of text to another user's terminal. It is mostly used to send urgent or important messages to other users. 

Syntax: 

write [username] [message]

Type "write" followed by the username of the recipient you want to send a message to. Then, type the message you want to send in quotes or without quotes.

Example:

To send a message to the user named "john", you would type: 

write john "Hey, are you available for a quick chat right now?"

After hitting enter, the message will be immediately sent to the user's terminal.

Note:

Before using the "write" command, make sure the recipient is currently logged in and their terminal is active. The recipient can also choose to decline the message by pressing Ctrl+D. 

## tldr 
 
> Write a message on the terminal of a specified logged in user (ctrl-C to stop writing messages).
> Use the `who` command to find out all terminal_ids of all active users active on the system. See also `mesg`.
> More information: <https://manned.org/write>.

- Send a message to a given user on a given terminal id:

`write {{username}} {{terminal_id}}`

- Send message to "testuser" on terminal `/dev/tty/5`:

`write {{testuser}} {{tty/5}}`

- Send message to "johndoe" on pseudo terminal `/dev/pts/5`:

`write {{johndoe}} {{pts/5}}`
