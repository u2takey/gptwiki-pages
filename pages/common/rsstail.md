# rsstail 
## chatgpt 
rsstail is a command-line utility that is used to monitor RSS (Really Simple Syndication) feeds for updates. It works by continuously checking the specified RSS feeds for new items and displaying them in real-time on the console.

The command syntax for rsstail is:

rsstail [options] url [url2 ...]

Here, options refer to various runtime options that can be passed to the command, and url specifies the URL of the RSS feed to monitor.

Some of the common options that can be used with rsstail are:

-1, --once: Causes rsstail to check the feeds only once and then exit.

-f, --feed-info: Displays information about the feed such as its title, description, and author.

-s, --summary: Displays a summary of each item in the feed.

-c, --content: Displays the full content of each item in the feed.

-u, --user-agent: Specifies the user-agent string to use for HTTP requests.

-i, --ignore-errors: Ignores any errors that occur while processing the feed.

-p, --pretend: Only displays the feed items that would be updated but does not actually update them.

Once the command is executed, rsstail starts monitoring the specified RSS feed(s) and displays any new items in real-time on the console. The output can be customized using the available options to suit the user's preferences. 

## tldr 
 
> `tail` for RSS feeds.
> More information: <https://github.com/gvalkov/rsstail.py>.

- Show the feed of a given URL and wait for new entries appearing at the bottom:

`rsstail -u {{url}}`

- Show the feed in reverse chronological order (newer at the bottom):

`rsstail -r -u {{url}}`

- Include publication date and link:

`rsstail -pl -u {{url}}`

- Set update interval:

`rsstail -u {{url}} -i {{interval_in_seconds}}`

- Show feed and exit:

`rsstail -1 -u {{url}}`
