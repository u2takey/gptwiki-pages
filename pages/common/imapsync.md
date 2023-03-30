# imapsync 
## chatgpt 
imapsync is a command-line tool that is primarily used for migrating email accounts from one email server to another. It is a powerful tool that can copy all email messages, contacts, calendars, and other data from one server to another while preserving the folder structure, message flags, and other metadata associated with each message.

The imapsync command takes several arguments, including the source email server and account information, the destination email server and account information, and various options that control how the migration process works. Some of the key options that can be specified with the imapsync command include:

- --host1 and --user1: These options specify the hostname and account name of the source email server that contains the email messages to be migrated.

- --host2 and --user2: These options specify the hostname and account name of the destination email server where the email messages will be copied to.

- --password1 and --password2: These options specify the password for the source and destination email accounts, respectively.

- --syncinternaldates: This option tells imapsync to preserve the original date and time of each email message when it is copied to the destination server.

- --skipsize: This option skips copying the size of the messages and associated metadata.

- --ssl1 and --ssl2: These options specify whether SSL should be used when connecting to the source and destination email servers.

In addition to these options, there are many other flags and parameters that can be passed to the imapsync command depending on the specific needs of the migration project. Overall, imapsync is a powerful and flexible tool that can help simplify the process of migrating email messages from one server to another while preserving important metadata and message structure. 

## tldr 
 
> Email IMAP tool for syncing, copying and migrating email mailboxes between two IMAP servers, one way, and without duplicates.
> More information: <https://imapsync.lamiral.info>.

- Synchronize IMAP account between host1 and host2:

`imapsync --host1 {{host1}} --user1 {{user1}} --password1 {{secret1}} --host2 {{host2}} --user2 {{user2}} --password2 {{secret2}}`
