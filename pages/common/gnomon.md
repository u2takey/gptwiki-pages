# gnomon 
## chatgpt 
The "gnomon" command is a third-party tool that adds a visual aid to the terminal shell. When executed, it displays a small, semi-transparent clock that sits atop the standard terminal output of other commands. The clock provides a clear reference point for when the command was executed and how long it took to complete.

The "gnomon" command is typically used for long-running tasks like backups, data imports, or large file transfers. By using gnomon, users can keep track of the progress of the task and estimate its completion time.

To use the "gnomon" command, you need to have it installed on your system. The installation process may vary depending on the operating system, but is generally straightforward. Once installed, simply execute the "gnomon" command followed by the command you want to run.

For example, to use gnomon alongside the "ping" command, you would run:

```
gnomon ping google.com
```

This would execute the "ping" command and display output as usual, but with the addition of the transparent clock at the top. As the ping command executes, the clock will update to provide a visual estimate of how long the process will take to complete.

In summary, the "gnomon" command provides a useful visual aid for long-running terminal commands in order to better track their progress and completion time. 

## tldr 
 
> Utility to annotate console logging statements with timestamps and find slow processes.
> More information: <https://github.com/paypal/gnomon>.

- Use UNIX (or DOS) pipes to pipe the `stdout` of any command through gnomon:

`{{npm test}} | gnomon`

- Show number of seconds since the start of the process:

`{{npm test}} | gnomon --type=elapsed-total`

- Show an absolute timestamp in UTC:

`{{npm test}} | gnomon --type=absolute`

- Set a high threshold of 0.5 seconds for the elapsed time; exceeding which the timestamp will be colored bright red:

`{{npm test}} | gnomon --high {{0.5}}`

- Set a medium threshold of 0.2 seconds (Timestamp will be colored bright yellow):

`{{npm test}} | gnomon --medium {{0.2}}`
