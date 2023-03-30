# irssi 
## chatgpt 
Irssi is a popular command-line based chat client used for connecting to IRC (Internet Relay Chat) networks. The name "Irssi" derives from the word "irssistible," which means "powerful" in Finnish. 

When executed on a Linux or Unix system, the "irssi" command starts the Irssi application, which displays a terminal-based user interface for interacting with IRC networks. 

Using Irssi, users can join different channels, communicate with others over text chat, share files, and receive various notifications such as system messages, highlights, and private messages. 

To use Irssi, you'll need to know the basic commands for navigating and interacting with the application. For example, some of the most commonly used commands include: 

- /server : This command is used to connect to an IRC server.

- /join : This command is used to join an IRC channel.

- /part : This command is used to leave an IRC channel.

- /msg : This command is used to send a private message to another user on the IRC network.

- /who : This command is used to view the list of users currently present on an IRC channel.

Overall, Irssi is a powerful command-line client that is popular among Linux and Unix users for its simplicity, flexibility, and customizability. 

## tldr 
 
> Text based IRC client.
> More information: <https://irssi.org>.

- Open Irssi and connect to a server with a nickname:

`irssi -n {{nickname}} -c {{irc.example.com}}`

- Open Irssi and connect with a specific server on a given port:

`irssi -c {{irc.example.com}} -p {{port}}`

- View the help:

`irssi --help`

- Join a channel:

`/join {{#channelname}}`

- Change active window (starts at 1):

`/win {{window_number}}`

- Exit the application cleanly and quitting any server(s):

`/quit`
