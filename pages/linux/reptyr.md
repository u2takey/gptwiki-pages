# reptyr 
## chatgpt 
reptyr is a command-line tool used in Unix or Unix-like operating systems that allows a user to redirect the input and output streams of an already running process to a different terminal. This means that you can take a program that has already started running in one terminal window and attach it to another terminal window, without having to restart the program or losing any of its data.

The command syntax for reptyr is as follows:

```
reptyr <pid>
```

Here, `<pid>` is the process ID of the program that you want to re-attach to a different terminal window. 

To use reptyr, you must first determine the `<pid>` of the program that you want to re-attach. You can do this by running the `ps` command, which shows a list of all running processes on your system along with their IDs. Once you have the `<pid>` of the process that you want to re-attach, simply run the `reptyr` command with that `<pid>` as an argument.

When you run reptyr with a `<pid>`, it will attach to the running process and redirect its input and output streams to your current terminal window. From here, you can interact with the program just as you would if you had started it in the current terminal window. You can also detach from the program at any time by pressing the Ctrl+C key combination.

In summary, reptyr is a tool that allows you to re-attach a running program to a different terminal window, without having to restart the program or losing any of its data. 

## tldr 
 
> Move a running process to a new terminal.
> Best used when you forget to start a long running task in `screen`.
> More information: <https://github.com/nelhage/reptyr>.

- Move a running process to your current terminal:

`reptyr {{pid}}`
