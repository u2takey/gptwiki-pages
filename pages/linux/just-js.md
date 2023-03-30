# just 
## chatgpt 
The "just" command doesn't have much to explain as it is not a pre-installed command in most operating systems. It is a command-line tool developed by the Swift community that helps to simplify running commands within a project. 

It enables users to define a set of tasks through a configuration file and execute them via the command line. These tasks could be arbitrary shell commands, commonly used project commands, or even custom scripts.

The "just" command also supports task dependencies and parallel execution, making it a powerful tool for complex build configurations.

Just basic syntax:
$ just [task_name]  # Runs the specified task. 
$ just --list      # Lists all available tasks. 
$ just --version   # Displays version information.

Overall, it is a useful tool for developers working on large or complex projects, simplifying the command-line interface and improving productivity. 

## tldr 
 
> A V8 JavaScript runtime for Linux.
> More information: <https://github.com/just-js/just>.

- Start a REPL (interactive shell):

`just`

- Run a JavaScript file:

`just {{path/to/file.js}}`

- Evaluate JavaScript code by passing it as an argument:

`just eval "{{code}}"`

- Initialize a new project in a directory of the same name:

`just init {{project_name}}`

- Build a JavaScript application into an executable:

`just build {{path/to/file.js}} --static`
