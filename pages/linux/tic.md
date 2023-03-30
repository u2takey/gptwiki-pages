# tic 
## chatgpt 
The "tic" command is a basic command used in MATLAB programming language. When executed, it starts a timer that is used to measure the elapsed time for a specific operation or process. 

The syntax for the "tic" command is straightforward – it is simply "tic". When it is called, the command waits for a signal to start timing. The signal can be initiated by calling the "toc" command, which stops the timer and returns the elapsed time from the "tic" command's execution to the call of the "toc" command in seconds. 

The "tic" command is used to measure the execution time of code blocks or functions and is useful for debugging, performance optimization, and benchmarking code. It can be used in conjunction with other commands like fprintf, to print out the elapsed time when a particular code block or function completes its execution. 

Overall, the "tic" command is a simple yet essential tool in MATLAB that helps developers measure the performance of their code in terms of speed and also identify areas that can be optimized. 

## tldr 
 
> Compile terminfo and install for ncurses.
> More information: <https://pubs.opengroup.org/onlinepubs/007908799/xcurses/terminfo.html>.

- Compile and install terminfo for a terminal:

`tic -xe {{terminal}} {{path/to/terminal.info}}`

- Check terminfo file for errors:

`tic -c {{path/to/terminal.info}}`

- Print database locations:

`tic -D`
