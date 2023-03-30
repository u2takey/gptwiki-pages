# nodemon 
## chatgpt 
nodemon is a command line utility that helps developers in automatically restarting the node.js application when any changes are detected in the source code of the application. 

Here's a detailed explanation of the nodemon command:

- nodemon: It's the basic command to start the nodemon utility.
- The utility starts watching the changes in the specified files and directories by default. If any changes occur, nodemon restarts the application automatically.
- Developers can specify the entry point of the application, the file that invokes the node.js server with the -e, --exec flag.
- Developers can exclude the files or directories from watching with the -i, --ignore flag.
- Developers can specify the environment variables with the -e, --env flag.
- Developers can specify the initial delay, before the first restart or before the subsequent restar with the -d, --delay flag.
- Developers can get the list of available options with the --help flag.

Overall, nodemon helps developers to improve the development experience by reducing the amount of time spent on manually restarting the node.js application while working on the code. 

## tldr 
 
> Watch files and automatically restart a node application when changes are detected.
> More information: <https://nodemon.io>.

- Execute the specified file and watch a specific file for changes:

`nodemon {{path/to/file.js}}`

- Manually restart nodemon (note nodemon must already be active for this to work):

`rs`

- Ignore specific files:

`nodemon --ignore {{path/to/file_or_directory}}`

- Pass arguments to the node application:

`nodemon {{path/to/file.js}} {{arguments}}`

- Pass arguments to node itself if they're not nodemon arguments already (e.g. `--inspect`):

`nodemon {{arguments}} {{path/to/file.js}}`

- Run an arbitrary non-node script:

`nodemon --exec "{{command_to_run_script}} {{options}}" {{path/to/script}}`

- Run a Python script:

`nodemon --exec "python {{options}}" {{path/to/file.py}}`
