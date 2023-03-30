# jtbl 
## chatgpt 
I'm sorry, but I cannot provide information on the command "jtbl" as it does not exist in commonly used programming or operating systems. Can you please clarify which context or programming language you are referring to? 

## tldr 
 
> Utility to print JSON and JSON Lines data as a table in the terminal.
> More information: <https://github.com/kellyjonbrazil/jtbl>.

- Print a table from JSON or JSON Lines input:

`cat {{file.json}} | jtbl`

- Print a table and specify the column width for wrapping:

`cat {{file.json}} | jtbl --cols={{width}}`

- Print a table and truncate rows instead of wrapping:

`cat {{file.json}} | jtbl -t`

- Print a table and don't wrap or truncate rows:

`cat {{file.json}} | jtbl -n`
