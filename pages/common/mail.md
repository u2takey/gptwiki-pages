# mail 
## chatgpt 
The "mail" command is a utility on Unix and Linux systems that allows users to send and receive email messages from the command line.

Here are some of the most common ways to use the mail command:

1. Sending an email message: 

To send an email message using the mail command, you need to use the following syntax:

`mail recipient@example.com`

After running this command, the mail command will wait for the user to input the message text. Once the message has been completed, the user can press "CTRL-D" to send the message.

2. Reading emails:

To read emails using the mail command, you can use the following syntax:

`mail`

This will display a list of all the emails in the user's inbox. Users can navigate through the emails using the arrow keys or the "N" and "P" keys. To read a specific email, users can select it from the list and then press "Enter".

3. Deleting emails:

To delete an email message from the inbox, users can follow these steps:

a. Open the inbox using the "mail" command.

b. Select the email that needs to be deleted.

c. Press the "d" key to flag the message for deletion.

d. Once all messages have been flagged, press "q" to quit the "mail" command.

4. Searching for emails:

To search for specific emails in the inbox, users can use the following syntax:

`mail -e search-term`

This will display all emails that match the search term. Users can then select the email they want to read using the arrow keys or the "N" and "P" keys.

Overall, the mail command is a versatile and powerful tool for managing email messages from the command line. Its simplicity and flexibility make it a popular choice among users who prefer to work with text-based interfaces. 

## tldr 
 
> The command operates on the user's mailbox if no argument is given.
> To send an email the message body is built from standard input.
> More information: <https://manned.org/mail>.

- Send a typed email message. The command-line below continues after pressing Enter key. Input CC email-id (optional) press Enter key. Input message text (can be multiline). Press Ctrl-D key to complete the message text:

`mail --subject="{{subject line}}" {{to_user@example.com}}`

- Send an email that contains file content:

`mail --subject="{{$HOSTNAME filename.txt}}" {{to_user@example.com}} < {{path/to/filename.txt}}`

- Send a `tar.gz` file as an attachment:

`tar cvzf - {{path/to/directory1 path/to/directory2}} | uuencode {{data.tar.gz}} | mail --subject="{{subject_line}}" {{to_user@example.com}}`
