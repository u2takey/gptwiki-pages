# mutt 
## chatgpt 
Mutt is a text-based email client for Unix-like systems. It allows users to read and send email messages from within a terminal window.

When you enter the command "mutt" from the terminal, the program launches and presents you with a prompt where you can enter various commands. Here are some of the most common commands in mutt:

- "m": Compose a new email message
- "r": Reply to the current message
- "f": Forward the current message
- "d": Delete the current message
- "u": Undelete the most recently deleted message
- "s": Save the current message in a file
- "q": Quit mutt

In addition to these basic commands, mutt also has a wide range of configuration options that can be customized in the ".muttrc" configuration file. These options allow you to change the appearance and behavior of the program to better suit your needs. For example, you can change the default editor to use when composing messages, or set up custom macros to automate common tasks.

Overall, mutt is a powerful and flexible email client that is well-suited for advanced users who prefer a text-based interface. 

## tldr 
 
> Command-line email client.
> More information: <http://mutt.org>.

- Open the specified mailbox:

`mutt -f {{mailbox}}`

- Send an email and specify a subject and a cc recipient:

`mutt -s {{subject}} -c {{cc@example.com}} {{recipient@example.com}}`

- Send an email with files attached:

`mutt -a {{file1}} {{file2}} -- {{recipient@example.com}}`

- Specify a file to include as the message body:

`mutt -i {{path/to/file}} {{recipient@example.com}}`

- Specify a draft file containing the header and the body of the message, in RFC 5322 format:

`mutt -H {{path/to/file}} {{recipient@example.com}}`
