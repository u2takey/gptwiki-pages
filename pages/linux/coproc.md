# coproc 
## chatgpt 
The `coproc` command is used in the Bash shell to create a co-process. A co-process allows communication between two shells or scripts, where one process sends data to the other for processing. 

The general syntax of the command is:

```
coproc <command>
```

Here, `<command>` is any shell command or script that is to be executed as a co-process.

When the `coproc` command is executed, a new process is created for the specified command. This process runs without any input or output streams attached to the console. Instead, the input and output streams of this process are connected to a pair of file descriptors.

The file descriptors are automatically created by the `coproc` command and assigned to two variables - `COPROC_IN` and `COPROC_OUT`. These variables can be used to read from and write to the co-process.

For example, consider the following script:

```
#!/bin/bash

coproc myproc {
   echo "This is myproc"
   read input
   echo "Input received: $input"
}

echo "Waiting for input..."
echo "Enter something: "
read output <&${myproc[0]}
echo "Received output: $output"
echo "Done"
```

Here, the `coproc` command is used to create a new co-process named "myproc". This process first prints "This is myproc" to its output stream, and then waits for input from the input stream.

In the main script, we read from the input stream of the co-process using the file descriptor `${myproc[0]}`. Whatever we enter as input is read by the co-process and printed back to the console as "Input received: ...".

The output of the co-process can also be captured in a variable using the output stream file descriptor `${myproc[1]}`. For example:

```
#!/bin/bash

coproc myproc {
   echo "This is myproc"
   read input
   echo "Input received: $input"
   echo "Output from myproc"
}

echo "Waiting for input..."
echo "Enter something: "
read output <&${myproc[0]}
echo "Received output: $output"
read proc_output <&${myproc[1]}
echo "Received proc output: $proc_output"
echo "Done"
```

Here, we have added a new line to the co-process, which simply prints "Output from myproc" to its output stream. In the main script, we read from the input and output streams of the co-process, using `${myproc[0]}` and `${myproc[1]}` file descriptors respectively. The output from the co-process is captured in the `proc_output` variable.

Overall, the `coproc` command is a powerful tool for inter-process communication in Bash, and is often used in complex shell scripts to manage multiple processes and streams of data. 

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

- Create a coprocess which repeatedly reads `stdin`, runs a pipeline on the input, and writes the output to `stdout`:

`coproc {{name}} { while read line; do echo "$line" | {{command1 | command2 | ...}} | cat /dev/fd/0; done }`

- Create and use a coprocess running `bc`:

`coproc BC { bc --mathlib; }; echo "1/3" >&"${BC[1]}"; read output <&"${BC[0]}"; echo "$output"`
