# script 
## chatgpt 
The `script` command is a Linux command that is used to generate a typescript of a terminal session. It records all input and output from the terminal, including commands entered by the user and messages produced by the system.

When you enter the `script` command in a terminal, it starts recording everything that is typed in the terminal session until you exit the session or type "exit". By default, the typescript is saved to a file named typescript in the current directory. You can specify a different filename by providing it as an argument to the command.

The `script` command is useful for documenting terminal sessions or for debugging purposes. It can help you keep track of what you did in a particular session and what commands you executed. You can also use it to create a log of a terminal session for later analysis or review.

To stop recording the terminal session, you just have to type "exit" or press Ctrl + D. Once you exit the session, the typescript file is closed, and you can view it in your favorite text editor or use other command-line tools to process the data. 

## tldr 
 
> Record all terminal output to file.
> More information: <https://manned.org/script>.

- Record a new session to a file named `typescript` in the current directory:

`script`

- Record a new session to a custom filepath:

`script {{path/to/session.out}}`

- Record a new session, appending to an existing file:

`script -a {{path/to/session.out}}`

- Record timing information (data is outputted to the standard error):

`script -t 2> {{path/to/timingfile}}`
