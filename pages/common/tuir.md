# tuir 
## chatgpt 
Tuir is a command that launches a text-based interface for browsing and interacting with the content of social news aggregator website Reddit. The name "tuir" stands for "Text User Interface Reddit". The tool provides a keyboard-driven UI for navigating and managing Reddit content, which includes subreddits, posts, comments, and user profiles.

Once launched, tuir presents a menu with a set of options that allow the user to log in to their Reddit account, browse the front page or a specific subreddit, search for posts or comments, view comments on a post, and interact with content by upvoting/downvoting, saving, or hiding it. The tool also offers some advanced features such as customizable key bindings, filtering options, and the ability to browse Reddit while offline.

Overall, tuir is a useful tool for Reddit power users who prefer a command-line interface over a web-based UI. It offers a lightweight, fast, and customizable way to explore and engage with the wide variety of content available on Reddit. 

## tldr 
 
> A text user-interface (TUI) to view and interact with Reddit from your terminal.
> Navigate with the Vim keys.
> More information: <https://gitlab.com/ajak/tuir>.

- Launch tuir:

`tuir`

- Open a subreddit:

`/{{subreddit_name}}`

- Open a link:

`o`

- Open a specific subreddit on launch:

`tuir -s {{subreddit_name}}`

- Open external links using programs defined in the mailcap config:

`tuir --enable-media`
