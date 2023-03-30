# mkfifo 
## chatgpt 
The `mkfifo` command is used to create a named pipe, also known as a FIFO (First In First Out) in a Unix-based system. A named pipe is a special type of file used for inter-process communication between two or more processes. 

The syntax of `mkfifo` command is:

```shell
mkfifo [options] filename
```

Where options are optional flags that can be used with the command, and filename is the name of the named pipe to be created.

Some common options used with `mkfifo` command are:

- `-m mode`: sets the file permissions for the named pipe. For example, `-m 777` sets read, write, and execute permissions for all users.
- `-v`: verbose mode, displays a message when the named pipe is created.

For example, the following command creates a named pipe named `myfifo`:

```shell
mkfifo myfifo
```

Once the named pipe is created, it can be used by two or more processes to communicate with each other. One process can write data to the named pipe, and another process can read that data from the pipe. 

For example, to write data to a named pipe, you can use the `echo` command:

```shell
echo "Hello world" > myfifo
```

And to read data from the named pipe, you can use the `cat` command:

```shell
cat myfifo
``` 

Overall, the `mkfifo` command is used to create a named pipe, which is a special type of file used for inter-process communication between two or more processes. 

## tldr 
 
> Makes FIFOs (named pipes).
> More information: <https://www.gnu.org/software/coreutils/mkfifo>.

- Create a named pipe at a given path:

`mkfifo {{path/to/pipe}}`
