# coproc 
## chatgpt 
The "coproc" command is used in Bash scripting to create a co-process or a child process that runs concurrently with the main process while sharing the same inputs and outputs. A co-process is a form of inter-process communication (IPC) that allows multiple processes to interact with each other in real-time.

The syntax of the "coproc" command is as follows:

```
coproc [name] command [redirects]
```

Where,
- `name`: Name of the co-process (optional)
- `command`: The command to be run as a co-process
- `redirects`: Specifies input, output, and error redirection for the co-process (optional)

When the "coproc" command is executed, Bash creates a pipe and forks a new process. The new process runs the specified command, and its input and output are redirected to the pipe. The pipe's file descriptors are then associated with the co-process name, making the co-process accessible from the main process.

The co-process can be used to perform tasks concurrently with the main process. For example, you can use a co-process to read data from a file, while the main process processes the data already read.

Once the co-process is created, Bash assigns it a unique identifier in the form of an array variable. The variable name is the name of the co-process followed by a set of parentheses. The variable contains two file descriptors representing the input and output of the co-process. You can use these file descriptors to send commands and receive output from the co-process.

To terminate the co-process, you can use the "kill" command with the process ID of the co-process.

In summary, the "coproc" command is a useful way to create a co-process that can run concurrently with the main process while sharing the same inputs and outputs. It can be used for inter-process communication and parallel processing in Bash scripts. 

## tldr 
 
> Bash builtin for creating interactive asynchronous subshells.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#Coprocesses>.

- Run a subshell asynchronously:

`coproc { {{command1; command2; ...}}; }`

- Create a coprocess with a specific name:

`coproc {{name}} { {{command1; command2; ...}}; }`

- Write to a specific coprocess `stdin`:

`echo "{{input}}" >&"${{{name}}[1]}"`

- Read from a specific coprocess `stdout`:

`read {{variable}} <&"${{{name}}[0]}"`

- Create a coprocess which repeatedly reads `stdin` and runs some commands on the input:

`coproc {{name}} {  while read line; do {{command1; command2; ...}}; done }`

- Create and use a coprocess running `bc`:

`coproc BC { bc --mathlib; }; echo "1/3" >&"${BC[1]}"; read output <&"${BC[0]}"; echo "$output"`
