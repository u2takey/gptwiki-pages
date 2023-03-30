# abduco 
## chatgpt 
abduco is a command-line tool used for managing long-running terminal sessions (or "abductions"). It works as a session manager for TUI (Text User Interface) programs and allows you to detach and reattach from terminal sessions.

Here's a brief description of some of the common flags and options used with the abduco command:

- -c <cmd>: execute the given command in the abduco session
- -e <env>: set the environment variable for the abduco session
- -A: attach to the last detached session
- -R: respawn and reattach to a session
- -r: reattach to a detached session
- -d <dir>: specify the directory to start the session in

To use abduco, you first need to start a new session with the "abduco -c" command, followed by the TUI program you want to run. For example, to start a session with the vim editor:

```
abduco -c vim
```

Once the session is started, you can detach from it by pressing CTRL-\ followed by the character 'd'. This will leave the TUI program running in the background and return you to the terminal prompt.

To reattach to the session later, use the "abduco -r" command:

```
abduco -r
```

This will restore the TUI program and allow you to continue working where you left off. 

## tldr 
 
> Terminal session manager.
> More information: <http://www.brain-dump.org/projects/abduco/>.

- List sessions:

`abduco`

- Attach to a session, creating it if it doesn't exist:

`abduco -A {{name}} {{bash}}`

- Attach to a session with `dvtm`, creating it if it doesn't exist:

`abduco -A {{name}}`

- Detach from a session:

`Ctrl + \`

- Attach to a session in read-only mode:

`abduco -Ar {{name}}`
