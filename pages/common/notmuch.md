# notmuch 
## chatgpt 
Notmuch is a command-line interface tool that enables users to efficiently search, sort, and filter email messages in their mail archives. The command allows users to easily find and sort through their email messages using keywords, dates, sender, recipients, and other relevant criteria.

In particular, notmuch allows users to perform complex email searches that can filter messages based on text contents, tags, and threading, among other aspects. This means that users can quickly locate specific emails, groups of emails, or sets of emails that match their search criteria with just a few simple commands.

Notmuch also enables users to tag their email messages for easier organization and classification. They can use tags to mark individual messages, threads, or sets of messages with customized labels that reflect their content, status, or importance.

Overall, notmuch provides users with a powerful tool for managing their email messages from the command line, thereby simplifying and expediting the email management process. 

## tldr 
 
> Command-line based program for indexing, searching, reading, and tagging large collections of email messages.
> More information: <https://notmuchmail.org/manpages/>.

- Configure for first use:

`notmuch setup`

- Add a tag for all messages matching a search term:

`notmuch tag +{{custom_tag}} "{{search_term}}"`

- Remove a tag for all messages matching a search term:

`notmuch tag -{{custom_tag}} "{{search_term}}"`

- Count messages matching the given search term:

`notmuch count --output={{messages|threads}} "{{search_term}}"`

- Search for messages matching the given search term:

`notmuch search --format={{json|text}} --output={{summary|threads|messages|files|tags}} "{{search_term}}"`

- Limit the number of search results to X:

`notmuch search --format={{json|text}} --output={{summary|threads|messages|files|tags}} --limit={{X}} "{{search_term}}"`

- Create a reply template for a set of messages:

`notmuch reply --format={{default|headers-only}} --reply-to={{sender|all}} "{{search_term}}"`
