# sendmail 
## chatgpt 
Sendmail is a popular mail transfer agent (MTA) used for delivering email messages from a client's machine to the recipient's server. It is an open-source software that is widely used on Unix and Linux systems.

The Sendmail command is used to start, stop, and manage the Sendmail daemon. The Sendmail daemon is responsible for transferring email from the user's machine to the recipient's server using the SMTP protocol.

The Sendmail command can be used to perform various tasks such as:

1. Starting the Sendmail daemon: The command `service sendmail start` or `service sendmail restart` can be used to start the sendmail daemon.

2. Stopping the Sendmail daemon: The command `service sendmail stop` can be used to stop the sendmail daemon.

3. Configuring Sendmail: Sendmail can be configured using the configuration file `sendmail.cf`. The command `sendmailconfig` can be used to configure Sendmail.

4. Testing Sendmail: The command `sendmail -bv <email address>` can be used to test Sendmail. This command verifies whether the email address is valid or not.

5. Sending email: The command `sendmail <recipient email address>` can be used to send an email to the recipient.

In summary, Sendmail is a powerful and flexible mail transfer agent that allows users to send emails from their machine. The Sendmail command is used to manage and configure the Sendmail daemon to ensure efficient email delivery. 

## tldr 
 
> Send email from the command-line.
> More information: <https://manned.org/sendmail>.

- Send a message with the content of `message.txt` to the mail directory of local user `username`:

`sendmail {{username}} < {{message.txt}}`

- Send an email from you@yourdomain.com (assuming the mail server is configured for this) to test@gmail.com containing the message in `message.txt`:

`sendmail -f {{you@yourdomain.com}} {{test@gmail.com}} < {{message.txt}}`

- Send an email from you@yourdomain.com (assuming the mail server is configured for this) to test@gmail.com containing the file `file.zip`:

`sendmail -f {{you@yourdomain.com}} {{test@gmail.com}} < {{file.zip}}`
