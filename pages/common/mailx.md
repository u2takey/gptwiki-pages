# mailx 
## chatgpt 
The mailx command is used to send and receive emails from the command line in Unix-like operating systems. When the mailx command is used without any arguments, it opens a new email message in the default text editor for the user to compose an email. Here are some frequently used options and arguments for the mailx command:

- -s: Specifies the subject line of the email message. For example, "mailx -s 'Hello World' user@example.com" would send an email to user@example.com with the subject "Hello World".
- -a: Attaches a file to the email message. This option is followed by the filename of the file to be attached. For example, "mailx -s 'Report' -a report.docx user@example.com" would attach the file report.docx to the email message with the subject "Report".
- -r: Specifies the email address of the sender. For example, "mailx -r myname@example.com -s 'Hello' user@example.com" would send an email from myname@example.com to user@example.com with the subject "Hello".
- -c: Sends a copy of the email message to the specified email address. For example, "mailx -s 'Hello' -c ccuser@example.com user@example.com" would send an email to user@example.com with the subject "Hello" and also send a copy to ccuser@example.com.
- -b: Sends a blind copy of the email message to the specified email address. For example, "mailx -s 'Hello' -b bccuser@example.com user@example.com" would send an email to user@example.com with the subject "Hello" and also send a blind copy to bccuser@example.com.

The mailx command can also be used to read and manage emails in a local mailbox or a remote server mailbox. To read emails, simply enter "mailx" without any arguments. The user will be presented with a list of emails in their mailbox. The user can then enter the number of the email they would like to read to view the email. The user can also use various commands to manage their mailbox, such as "q" to quit, "d" to delete an email, "u" to undelete an email, and "s" to save an email to a file. Overall, the mailx command is a powerful tool for sending and receiving emails directly from the command line. 

## tldr 
 
> Send and receive mail.
> More information: <https://manned.org/mailx>.

- Send mail (the content should be typed after the command, and ended with `Ctrl+D`):

`mailx -s "{{subject}}" {{to_addr}}`

- Send mail with content passed from another command:

`echo "{{content}}" | mailx -s "{{subject}}" {{to_addr}}`

- Send mail with content read from a file:

`mailx -s "{{subject}}" {{to_addr}} < {{content.txt}}`

- Send mail to a recipient and CC to another address:

`mailx -s "{{subject}}" -c {{cc_addr}} {{to_addr}}`

- Send mail specifying the sender address:

`mailx -s "{{subject}}" -r {{from_addr}} {{to_addr}}`

- Send mail with an attachment:

`mailx -a {{path/to/file}} -s "{{subject}}" {{to_addr}}`
