# stdbuf 
## chatgpt 
The `stdbuf` command is used to change the buffering applied to input and output streams of a program. 

The basic syntax of `stdbuf` is:

```
stdbuf [OPTIONS] COMMAND [ARGUMENTS]
```

Here, `OPTIONS` are optional arguments that can be used to specify the size of the buffer, the mode of the buffer, and so on. `COMMAND` is the command to be executed, and `ARGUMENTS` are the arguments to be passed to the command.

By default, input and output streams are buffered in most programs. The `stdbuf` command allows you to change the buffering behaviour so that data is transmitted as soon as it is available, rather than when a buffer is filled. This can be useful in situations where you want quick access to data, or when you want to avoid delays caused by buffering.

Some of the commonly used options of `stdbuf` are:

- `-i`: Sets input stream buffering to line buffered
- `-o`: Sets output stream buffering to line buffered
- `-e`: Sets error stream buffering to line buffered
- `-i0`, `-o0`, `-e0`: Disables buffering for input, output, and error streams, respectively

For example, to run a command with no output buffering, you can use:

```
stdbuf -o0 COMMAND
```

Similarly, to run a command with no input buffering, you can use:

```
stdbuf -i0 COMMAND
```

In conclusion, the `stdbuf` command is a useful tool to control the buffering behaviour of input and output streams of a program, making it easy to work with data in real-time. 

## tldr 
 
> Run a command with modified buffering operations for its standard streams.
> More information: <https://www.gnu.org/software/coreutils/stdbuf>.

- Change the standard input buffer size to 512 KiB:

`stdbuf --input={{512K}} {{command}}`

- Change the standard output buffer to line-buffered:

`stdbuf --output={{L}} {{command}}`

- Change the standard error buffer to unbuffered:

`stdbuf --error={{0}} {{command}}`
