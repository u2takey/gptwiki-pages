# msmtp 
## chatgpt 
msmtp is an SMTP (Simple Mail Transfer Protocol) client that can be used to send email messages from a command line or script. It can be used as a standalone program or in combination with other programs or scripts.

The basic syntax for using msmtp is as follows:

msmtp [options] recipient_email

The recipient_email is the email address of the recipient of the email message.

Some of the most commonly used options for msmtp are:

-h smtp_server – specifies the SMTP server to use for sending the message.

-f sender_email – specifies the email address of the sender of the message.

-a account_name – specifies the name of the account to use for authentication.

-u username – specifies the username to use for authentication.

-p password – specifies the password to use for authentication.

-t – specifies that the message should be sent to the recipients specified in the To: and Cc: headers of the message.

-i – specifies that the message should be sent in interactive mode, which allows the user to interactively enter the message.

These are just a few of the many options that can be used with msmtp. For a complete list of options, see the msmtp man page or help file. 

## tldr 
 
> An SMTP client.
> It reads text from standard input and sends it to an SMTP server.
> More information: <https://marlam.de/msmtp>.

- Send an email using the default account configured in `~/.msmtprc`:

`echo "{{Hello world}}" | msmtp {{to@example.org}}`

- Send an email using a specific account configured in `~/.msmtprc`:

`echo "{{Hello world}}" | msmtp --account={{account_name}} {{to@example.org}}`

- Send an email without a configured account. The password should be specified in the `~/.msmtprc` file:

`echo "{{Hello world}}" | msmtp --host={{localhost}} --port={{999}} --from={{from@example.org}} {{to@example.org}}`
