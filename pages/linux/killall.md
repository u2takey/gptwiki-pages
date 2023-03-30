# killall 
## chatgpt 
killall is a command that is used to terminate all running processes with a given name. The syntax of the command is simple: "killall  [process name]".

For instance, if we want to stop all running instances of the Firefox web browser, we can use the command "killall firefox". After executing this command, all running Firefox processes will be terminated.

This command can also be used with the option "-u" to stop all processes for a given user. In this case, the command would be "killall -u [username]".

One important thing to note is that the killall command will forcefully terminate all running processes with the given name or user. Therefore, it should be used with caution as it may lead to data loss and system instability. It's always recommended to save any unsaved work before running the killall command. 

## tldr 
 
> Send kill signal to all instances of a process by name (must be exact name).
> All signals except SIGKILL and SIGSTOP can be intercepted by the process, allowing a clean exit.
> More information: <https://manned.org/killall>.

- Terminate a process using the default SIGTERM (terminate) signal:

`killall {{process_name}}`

- List available signal names (to be used without the 'SIG' prefix):

`killall --list`

- Interactively ask for confirmation before termination:

`killall -i {{process_name}}`

- Terminate a process using the SIGINT (interrupt) signal, which is the same signal sent by pressing `Ctrl + C`:

`killall -INT {{process_name}}`

- Force kill a process:

`killall -KILL {{process_name}}`
