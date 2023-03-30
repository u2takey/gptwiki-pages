# r2e 
## chatgpt 
As an AI language model, I do not have enough context to provide a specific answer to your question about the command "r2e" as it could mean different things depending on the software or platform you are working with. However, here are some possible explanations:

- In the context of programming, "r2e" might be a custom command or function defined by a developer as an abbreviation for something else. In this case, it would be necessary to consult the code or documentation to know exactly what it does.
- "r2e" could also be an acronym or abbreviation for a specific software or tool. For example, "r2e" could refer to "RSS-to-email", a service that converts RSS feeds into email newsletters. In this case, using the command "r2e" would involve providing necessary information such as the RSS feed URL, email recipient, and formatting options.
- Alternatively, "r2e" might not be a recognized command at all on your system. If you try to execute it in a terminal or command prompt, you may get an error message indicating that the command is not found. In this case, you might try searching for the correct syntax or command to achieve what you need to do, or contact technical support for help. 

## tldr 
 
> Forwards RSS feeds to an email address.
> Requires a configured `sendmail` or smtp setup.
> More information: <https://github.com/rss2email/rss2email>.

- Create a new feed database that sends email to an email address:

`r2e new {{email_address}}`

- Subscribe to a feed:

`r2e add {{feed_name}} {{feed_URI}}`

- Send new stories to an email address:

`r2e run`

- List all feeds:

`r2e list`

- Delete a feed at a specified index:

`r2e delete {{index}}`
