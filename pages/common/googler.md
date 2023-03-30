# googler 
## chatgpt 
Googler is a command line tool that allows users to perform Google searches via the terminal. When invoked, the command prompts the user to enter their search query and then displays the results in the terminal output. 

The syntax for using googler is:
```
googler [flags] [search terms]
```

Optional flags can be included to modify the behavior of the search. Some common flags include:

- `-h`, `--help`: display help information and exit
- `-c`, `--count`: display the total number of search results (without displaying individual results)
- `-n`, `--number`: set the maximum number of search results to display
- `-w`, `--wiki`: search on Wikipedia instead of Google

After any optional flags are specified, the search terms themselves can be entered. These can be any text string, including multiple words or phrases. 

Googler then retrieves and displays the search results within the terminal window. Each result includes the page title, a brief description, and the URL. The results can then be navigated using the arrow keys, and pressing 'enter' will open the selected page in the default browser. 

Overall, googler is a handy command line tool for performing quick and efficient Google searches without leaving the terminal or opening a web browser. 

## tldr 
 
> Search Google from command-line.
> More information: <https://github.com/jarun/googler>.

- Search Google for a keyword:

`googler {{keyword}}`

- Search Google and open the first result in web browser:

`googler -j {{keyword}}`

- Show N search results (default 10):

`googler -n {{N}} {{keyword}}`

- Disable automatic spelling correction:

`googler -x {{keyword}}`

- Search one site for a keyword:

`googler -w {{site}} {{keyword}}`

- Show Google search result in JSON format:

`googler --json {{keyword}}`

- Perform in-place self-upgrade:

`googler -u`

- For more help in interactive mode:

`?`
