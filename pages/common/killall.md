# killall 
## chatgpt 
The `killall` command is a Linux/Unix command used to kill all active processes with a given name. The basic syntax of the `killall` command is:

```
killall [options] process-name
```

Here, `process-name` is the name of the process to kill. The `killall` command sends a signal to each process named `process-name`, causing it to terminate.

Options that can be used with the `killall` command include:

- `-e`: Signals only processes with an exact match to the given name.
- `-i`: Interactively asks for confirmation before killing each process.
- `-q`: Quiet mode. Doesn't print any error messages.
- `-s`: Send a specific signal to the process.

Some examples of using the `killall` command are:

```
$ killall httpd
```

This command will terminate all processes that are running under the name "httpd".

```
$ killall -SIGKILL firefox
```

This command will send a "kill" signal to all processes that are running under the name "firefox".

```
$ killall -e bash
```

This command will kill only the processes that have an exact match to the name "bash". 

## tldr 
 
> Send kill signal to all instances of a process by name (must be exact name).
> All signals except SIGKILL and SIGSTOP can be intercepted by the process, allowing a clean exit.
> More information: <https://manned.org/killall>.

- Terminate a process using the default SIGTERM (terminate) signal:

`killall {{process_name}}`

- [l]ist available signal names (to be used without the 'SIG' prefix):

`killall -l`

- Interactively ask for confirmation before termination:

`killall -i {{process_name}}`

- Terminate a process using the SIGINT (interrupt) signal, which is the same signal sent by pressing `Ctrl + C`:

`killall -INT {{process_name}}`

- Force kill a process:

`killall -KILL {{process_name}}`
