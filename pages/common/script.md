# script 
## chatgpt 
The "script" command in Linux is used to record a terminal session. It is useful for keeping a log of everything you type and see on the terminal, and you can later refer to this log for troubleshooting or to recreate a particular session.

The syntax of the "script" command is as follows:

```script [options] [output_file]```

The available options for the "script" command are:

- -a: Append the output to the file instead of overwriting it.
- -c command: Run the specified command and record the output.
- -f: Flush the output after each write.
- -q: Quiet mode. Suppress the startup and exit messages.
- -t: Timestamp each line of output.
- -V: Display the version of the script command.

The "output_file" argument specifies the name of the file in which the output will be saved. If it is not specified, the default file name is "typescript" in the current directory. 

Once the "script" command is executed, it will start recording the session and everything you type and see on the terminal will be saved to the specified file. When you are done, you can exit the recording by pressing "Ctrl-D" or typing "exit". 

The recorded session will include all the commands you typed, their output, and any error messages that were displayed on the terminal. It is important to note that this recording will not capture any graphical output, but only text that is displayed in the terminal. 

## tldr 
 
> Make a typescript file of a terminal session.
> More information: <https://manned.org/script>.

- Start recording in file named "typescript":

`script`

- Stop recording:

`exit`

- Start recording in a given file:

`script {{logfile.log}}`

- Append to an existing file:

`script -a {{logfile.log}}`

- Execute quietly without start and done messages:

`script -q {{logfile.log}}`
