# fswatch 
## chatgpt 
`fswatch` is a command line tool used to monitor file system events, such as file or directory creation, modification, or deletion. It allows you to easily track changes in directories or specific files, and can be used for tasks such as automatically rebuilding a project when changes are made, syncing files between locations, or triggering backups.

The basic syntax for using `fswatch` is:

```
fswatch [options] [directory or file]
```

Here, `[options]` can be used to configure various aspects of monitoring, such as the types of events to track, the polling interval, or the output format. `[directory or file]` specifies the location to monitor, and can be a single file or a directory.

For example, to monitor all files in the current directory and its subdirectories for any kind of change, you could use:

```
fswatch .
```

To only track changes to a specific file, you can specify its path:

```
fswatch /full/path/to/file.txt
```

You can also use advanced features such as regular expressions to filter out unwanted events or run custom scripts in response to specific events.

Overall, `fswatch` is a powerful and flexible tool for monitoring file system events, and can be a valuable asset in a wide range of development, testing, and maintenance tasks. 

## tldr 
 
> A cross-platform file change monitor.
> More information: <https://emcrisostomo.github.io/fswatch>.

- Run a Bash command on file creation, update or deletion:

`fswatch {{path/to/file}} | xargs -n 1 {{bash_command}}`

- Watch one or more files and/or directories:

`fswatch {{path/to/file}} {{path/to/directory}} {{path/to/another_directory/**/*.js}} | xargs -n 1 {{bash_command}}`

- Print the absolute paths of the changed files:

`fswatch {{path/to/directory}} | xargs -n 1 -I {} echo {}`

- Filter by event type:

`fswatch --event {{Updated|Deleted|Created}} {{path/to/directory}} | xargs -n 1 {{bash_command}}`
