# mu 
## chatgpt 
As an AI language model, I don't have a context to determine exactly what you are referring to with the command "mu". It could be a command in a specific programming language, a command in a Linux terminal or a Windows CMD prompt, or any number of other possibilities. 

If you provide more information about the context and environment in which the command is being used, I may be able to provide more detailed information about what it does and how it works. 

## tldr 
 
> Index and search emails from a local Maildir.
> More information: <https://man.cx/mu>.

- Initialize the email database, optionally specifying the Maildir directory and email addresses:

`mu init --maildir={{path/to/directory}} --my-address={{name@example.com}}`

- Index new emails:

`mu index`

- Find messages using a specific keyword (in message body, subject, sender, ...):

`mu find {{keyword}}`

- Find messages to Alice with subject `jellyfish` containing the words `apples` or `oranges`:

`mu find to:{{alice}} subject:{{jellyfish}} {{apples}} OR {{oranges}}`

- Find unread messages about words starting with `soc` (the `*` only works at the end of the search term) in the Sent Items folder:

`mu find 'subject:{{soc}}*' flag:{{unread}} maildir:'/{{Sent Items}}'`

- Find messages from Sam with attached images, between 2 KiB and 2 MiB, written in 2021:

`mu find 'mime:{{image/*}} size:{{2k..2m}} date:{{20210101..20211231}} from:{{sam}}`

- List contacts with `Bob` in either name or email address:

`mu cfind {{Bob}}`
