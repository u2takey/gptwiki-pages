# watch 
## chatgpt 
The `watch` command is a Linux/Unix command that allows you to monitor a command periodically and displays its output every few seconds. The syntax of the `watch` command is:

```
watch [options] command
```

Here, `command` is the command that you want to monitor or watch periodically.

The `watch` command repeats the command specified in the command line and displays its output on the terminal screen every 2 seconds by default, but you can change the interval using the `-n` option.

Some of the commonly used options with `watch` are:

- `-n <interval>`: Sets the interval in seconds at which the `watch` command repeats the command. For example, `watch -n 5 "ls -l"` will repeat the `ls -l` command every 5 seconds.
- `-d` or `--differences`: Highlights the differences between the previous and the current output of the command in a bold font.
- `-c` or `--color`: Enables color highlighting for the output.
- `-t` or `--no-title`: Hides the header showing the current time and interval.

The `watch` command is useful for monitoring the progress of long-running commands or scripts, checking the status of system services, and keeping track of system performance metrics. 

## tldr 
 
> Execute a program periodically, showing output fullscreen.
> More information: <https://manned.org/watch>.

- Repeatedly run a command and show the result:

`watch {{command}}`

- Re-run a command every 60 seconds:

`watch -n {{60}} {{command}}`

- Monitor the contents of a directory, highlighting differences as they appear:

`watch -d {{ls -l}}`

- Repeatedly run a pipeline and show the result:

`watch '{{command_1}} | {{command_2}} | {{command_3}}'`
