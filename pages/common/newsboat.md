# newsboat 
## chatgpt 
Newsboat is a command-line RSS feed reader for Linux, macOS, and BSD. It allows users to easily consume and manage their favorite RSS feeds from the terminal.

When executed, the newsboat command opens the Newsboat application in the terminal. From there, users can use various keyboard shortcuts and commands to navigate and manage their feeds. Some of the key features of Newsboat include:

- Offline reading: Newsboat can download and cache feed content, allowing users to read their feeds even when offline.
- Customization: Users can modify keybindings, colors, and other aspects of the application to suit their preferences.
- Security: Newsboat supports SSL/TLS encryption for secure feed fetching.
- Extensibility: Newsboat supports plugins and scripts to enable additional functionality.

Overall, the newsboat command provides a powerful and flexible way to consume RSS feeds from the command line. 

## tldr 
 
> An RSS/Atom feed reader for text terminals.
> More information: <https://newsboat.org/>.

- First import feed URLs from an OPML file:

`newsboat -i {{my-feeds.xml}}`

- Alternatively, add feeds manually:

`echo {{http://example.com/path/to/feed}} >> "${HOME}/.newsboat/urls"`

- Start newsboat and refresh all feeds on startup:

`newsboat -r`

- Execute a space-separated list of commands in non-interactive mode:

`newsboat -x {{reload print-unread ...}}`

- See keyboard shortcuts (the most relevant are visible in the status line):

`?`
