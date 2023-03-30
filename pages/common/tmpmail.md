# tmpmail 
## chatgpt 
Unfortunately, as an AI language model, I don't have access to your local system to describe the command "tmpmail" in detail. However, in general, "tmpmail" is a command-line tool for generating temporary email addresses that can be used to receive emails and verify online accounts without sharing your actual email address. The tool creates a disposable email address with a unique inbox and forwards all emails received to your actual email address. This can help protect your privacy and reduce spam in your primary inbox. 

The functionality and usage of "tmpmail" command may vary depending on the operating system and version being used. You could try running the "man tmpmail" command in your terminal to view the manual page for this tool which provides more detailed information about the usage and syntax of this command on your system. 

## tldr 
 
> A temporary email right from your terminal written in POSIX sh.
> More information: <https://github.com/sdushantha/tmpmail>.

- Create a temporary inbox:

`tmpmail --generate`

- List messages and their numeric ID:

`tmpmail`

- Display the most recent received email:

`tmpmail --recent`

- Open a specific message:

`tmpmail {{email_id}}`

- View email as raw text without HTML tags:

`tmpmail --text`

- Open email with a specific browser (default is w3m):

`tmpmail --browser {{browser}}`
