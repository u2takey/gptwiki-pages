# inotifywait 
## chatgpt 
`inotifywait` is a Linux command-line tool used to monitor file system events such as file creation, modification, or deletion. It is based on the `inotify` Linux kernel subsystem, which allows applications to monitor changes to a file or directory in real-time.

The command has the following syntax:

```
inotifywait [options] file/directory
```

Here, `options` refer to any additional flags or arguments passed to the command, and `file/directory` specifies the file or directory to be monitored.

When executed, `inotifywait` will sit in the background, waiting for any events that occur in the specified file or directory. When an event occurs, the command will print information about the event to the terminal. This information typically includes the type of event, the filename, and the timestamp.

Some of the commonly used options with `inotifywait` command are:

- `-r`: Monitor the specified directory recursively.
- `-m`: Keep monitoring for events continuously.
- `-e <event>`: Only monitor the specified event(s).
- `--format`: Specify the output format.

For example, the following command will monitor the directory `/var/log` for any changes:

```
inotifywait -r /var/log
```

This will display all the events that occur in `/var/log` on your terminal.

Overall, `inotifywait` is a powerful command-line tool that can help monitor file system events in real-time, making it useful for various tasks such as automated backups, logging changes, and more. 

## tldr 
 
> Waits for changes to one or more files.
> More information: <https://manned.org/inotifywait>.

- Watch a specific file for events, exiting after the first one:

`inotifywait {{path/to/file}}`

- Continuously watch a specific file for events without exiting:

`inotifywait --monitor {{path/to/file}}`

- Watch a directory recursively for events:

`inotifywait --monitor --recursive {{path/to/directory}}`

- Watch a directory for changes, excluding files, whose names match a regular expression:

`inotifywait --monitor --recursive --exclude "{{regular_expression}}" {{path/to/directory}}`

- Watch a file for changes, exiting when no event occurs for 30 seconds:

`inotifywait --monitor --timeout {{30}} {{path/to/file}}`

- Only watch a file for file modification events:

`inotifywait --event {{modify}} {{path/to/file}}`

- Watch a file printing only events, and no status messages:

`inotifywait --quiet {{path/to/file}}`

- Run a command when a file is accessed:

`inotifywait --event {{access}} {{path/to/file}} && {{command}}`
