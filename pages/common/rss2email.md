# rss2email 
## chatgpt 
The "rss2email" command is a tool used to retrieve RSS feeds and send them to an email address. It allows users to receive updates and news from their favorite websites or blogs directly in their email inbox. 

Here’s how the command works:

- First, the user needs to install the "rss2email" tool on their computer or server. This can be done using the appropriate package manager for their operating system, or by downloading and installing the tool manually.

- Once the tool is installed, the user can run the command with a set of parameters to configure it. The most important parameter is the RSS feed URL, which specifies the URL of the RSS feed that the user wants to subscribe to. The user can also specify other parameters, such as the email address to send the updates to, the frequency of updates, and the format of the emails.

- When the command is executed, the tool retrieves the latest updates from the RSS feed and sends them to the specified email address. The user can then read the updates and stay up-to-date with the latest news and content from their favorite websites.

Overall, the "rss2email" command is a useful tool for those who prefer to receive updates and news via email, rather than through a web browser or an RSS reader. It offers a simple and convenient way to stay informed and engaged with the content that matters most to them. 

## tldr 
 
> Tool for delivering news from RSS feeds to an email program.
> More information: <https://github.com/rss2email/rss2email>.

- List all feeds:

`r2e list`

- Convert RSS entries to email:

`r2e run`

- Add a feed:

`r2e add {{feed_address}}`

- Add a feed with a specific email address:

`r2e add {{feed_address}} {{new_email@example.com}}`

- Delete a specific feed:

`r2e delete {{number_of_feed_in_list}}`

- Display help:

`r2e -h`
