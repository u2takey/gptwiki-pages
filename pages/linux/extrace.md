# extrace 
## chatgpt 
I'm sorry, but "extrace" does not appear to be a valid command in any operating system or programming language. Can you please provide more information or context? 

## tldr 
 
> Trace exec() calls.
> More information: <https://github.com/chneukirchen/extrace>.

- Trace all program executions occurring on the system:

`sudo extrace`

- Run a command and only trace descendants of this command:

`sudo extrace {{command}}`

- Print the current working directory of each process:

`sudo extrace -d`

- Resolve the full path of each executable:

`sudo extrace -l`

- Display the user running each process:

`sudo extrace -u`
