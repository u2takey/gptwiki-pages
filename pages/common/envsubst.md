# envsubst 
## chatgpt 
The "envsubst" command is a Linux/Unix command that is used to substitute environment variables in a text file with their respective values. It takes a file as input and replaces all environment variable references in the file with their corresponding values.

The syntax for using the "envsubst" command is as follows:

```
envsubst [OPTIONS] [VARIABLE] [FILE]
```

Here, OPTIONS are any additional options that you can use with the command. VARIABLE refers to the environment variable that you want to substitute, and FILE is the name of the file that contains the environment variable references.

For example, let's say we have a file called "sample.txt" that contains the following text:

```
Hello $USER, your home directory is $HOME
```

To substitute the environment variables referenced in this file, we would use the command:

```
envsubst < sample.txt
```

This will produce the following output:

```
Hello your_username, your home directory is /home/your_username
```

Here, "$USER" has been replaced with the actual username, and "$HOME" has been replaced with the actual home directory.

Overall, the "envsubst" command is useful when you need to generate configuration files dynamically, especially when you need to include environment variables or variables that have been passed as command-line arguments. 

## tldr 
 
> Substitutes environment variables with their value in shell format strings.
> Variables to be replaced should be in either `${var}` or `$var` format.
> More information: <https://www.gnu.org/software/gettext/manual/html_node/envsubst-Invocation.html>.

- Replace environment variables in `stdin` and output to `stdout`:

`echo '{{$HOME}}' | envsubst`

- Replace environment variables in an input file and output to `stdout`:

`envsubst < {{path/to/input_file}}`

- Replace environment variables in an input file and output to a file:

`envsubst < {{path/to/input_file}} > {{path/to/output_file}}`

- Replace environment variables in an input file from a space-separated list:

`envsubst '{{$USER $SHELL $HOME}}' < {{path/to/input_file}}`
