# neomutt 
## chatgpt 
Neomutt is a command used to launch the neomutt email client application on a Linux or UNIX-based operating system. Neomutt is an advanced and highly configurable email client that can be customized to fit many different use cases and preferences.

When the neomutt command is executed, the application is launched and the user is presented with a command line interface for managing email. The neomutt interface provides a familiar email client experience, with options for composing new messages, replying to or forwarding existing messages, organizing email into folders, searching for specific messages, and more.

One of the key advantages of neomutt over other email clients is its flexibility and customization options. Users can configure neomutt to work with a wide range of email providers and protocols, and can customize the interface and behavior of the application to suit their specific needs.

Overall, the neomutt command is a powerful tool for managing email on a Linux or UNIX system, and is a popular choice for advanced users who value flexibility and customization options in their email client. 

## tldr 
 
> NeoMutt command line email client.
> More information: <https://neomutt.org>.

- Open the specified mailbox:

`neomutt -f {{path/to/mailbox}}`

- Start writing an email and specify a subject and a `cc` recipient:

`neomutt -s "{{subject}}" -c {{cc@example.com}} {{recipient@example.com}}`

- Send an email with files attached:

`neomutt -a {{path/to/file1 path/to/file2 ...}} -- {{recipient@example.com}}`

- Specify a file to include as the message body:

`neomutt -i {{path/to/file}} {{recipient@example.com}}`

- Specify a draft file containing the header and the body of the message, in RFC 5322 format:

`neomutt -H {{path/to/file}} {{recipient@example.com}}`
