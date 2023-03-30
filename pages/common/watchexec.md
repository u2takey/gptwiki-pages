# watchexec 
## chatgpt 
The watchexec command is a tool used to monitor file changes and execute commands in response to those changes. It is useful for automatically running tasks, compiling code, or updating files when changes are made.

The basic syntax of the watchexec command is as follows:

watchexec [option] [command]

Options:
- -w or --watch: A comma-separated list of files, directories or glob patterns to monitor
- -i or --ignore: A comma-separated list of files or directories to ignore
- -c or --clear: Clear the screen before executing the command
- -n or --interval: Set the interval at which the watch command checks for file changes (default is 100ms)
- -r or --restart: Restart the command on file changes instead of just reloading it
- -h or --help: Show the help menu
- -V or --version: Show the current version of watchexec

Examples:
1. watchexec -w src/main.js -c "node src/main.js"
This command monitors the src/main.js file for changes and executes the "node src/main.js" command when changes are detected.

2. watchexec -w src/ -i node_modules/ -c "npm run build"
This command monitors all files in the src directory, ignoring the node_modules directory, and executes the "npm run build" command when changes are detected.

Overall, the watchexec command is a powerful tool for automating tasks and keeping track of file changes in real-time. 

## tldr 
 
> Run arbitrary commands when files change.
> More information: <https://github.com/watchexec/watchexec>.

- Call `ls -la` when any file in the current directory changes:

`watchexec -- {{ls -la}}`

- Run `make` when any JavaScript, CSS and HTML files in the current directory change:

`watchexec --exts {{js,css,html}} make`

- Run `make` when any file in the `lib` or `src` subdirectories change:

`watchexec --watch {{lib}} --watch {{src}} {{make}}`

- Call/restart `my_server` when any file in the current directory change, sending `SIGKILL` to stop the child process:

`watchexec --restart --signal {{SIGKILL}} {{my_server}}`
