# goobook 
## chatgpt 
Goobook is a command-line tool for interacting with Google Contacts. The command provides a way to access and manage contacts stored in a Google account. With Goobook, users can add, delete, search, and modify contacts, as well as import and export contact information.

To use Goobook, first, open a command prompt or terminal window on your computer. Then, type "goobook" followed by a subcommand to perform a specific action. Some of the available subcommands include:

- "add": Adds a new contact to your Google account
- "delete": Removes a contact from your account
- "search": Finds a contact based on a specific keyword or phrase
- "edit": Modifies an existing contact's information
- "import": Imports contacts from a CSV or vCard file
- "export": Exports contacts to a CSV or vCard file

To use any of these subcommands, you need to authorize access to the Google Contacts API. Goobook will prompt you to grant permission to access your contacts upon the first use.

Overall, Goobook is a powerful tool for managing contacts in a Google account from the command line, providing a simple and efficient way to organize and maintain contact information. 

## tldr 
 
> Access Google contacts from `mutt` or the command line.
> More information: <https://manned.org/goobook>.

- Allow `goobook` to access Google contacts using OAuth2:

`goobook authenticate`

- Dump all contacts to XML (stdout):

`goobook dump_contacts`
