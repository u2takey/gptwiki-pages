# handlr 
## chatgpt 
I'm sorry, but "handlr" does not appear to be a valid command. It is possible that it is a misspelling or a command specific to a particular program or system. Can you provide more information on where you encountered this command? 

## tldr 
 
> Manage your default applications.
> More information: <https://github.com/chmln/handlr>.

- Open a URL in the default application:

`handlr open {{https://example.com}}`

- Open a PDF in the default PDF viewer:

`handlr open {{path/to/file.pdf}}`

- Set imv as the default application for PNG files:

`handlr set {{.png}} {{imv.desktop}}`

- Set MPV as the default application for all audio files:

`handlr set {{'audio/*'}} {{mpv.desktop}}`

- List all default apps:

`handlr list`

- Print the default application for PNG files:

`handlr get {{.png}}`
