# fortune 
## chatgpt 
The "fortune" command is a program available on Unix and Unix-like operating systems. It displays a random message or quote (known as "fortune") from a pre-installed database of sayings, jokes, quotes, and aphorisms. 

When the command is executed, it accesses a collection of text files containing various messages, often humorous or witty. The messages can be anything from well-known quotes to obscure sayings from books, movies, and TV shows.

The command accepts various options, such as "-a" to display all available fortunes, "-s" to suppress the display of ads and fortune headers, "-n" to specify the maximum length of the fortune, and "-m" to specify the file(s) containing fortunes to be accessed.

The "fortune" command is often used in scripts and terminal-based games to add a random element to the output. It can also be used for entertainment and inspiration, as well as to give users a break from tedious work routines. 

## tldr 
 
> Print a random quotation (fortune-cookie style).
> More information: <https://manned.org/fortune>.

- Print a quotation:

`fortune`

- Print an offensive quotation:

`fortune -o`

- Print a long quotation:

`fortune -l`

- Print a short quotation:

`fortune -s`

- List the available quotation database files:

`fortune -f`

- Print a quotation from one of the database files listed by `fortune -f`:

`fortune {{path/to/file}}`
