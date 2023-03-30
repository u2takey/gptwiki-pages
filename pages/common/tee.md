# tee 
## chatgpt 
The "tee" command is a Unix/Linux utility that reads the standard input and copies it to the standard output and to one or more files, effectively allowing a user to split the output of a command or pipeline onto multiple destinations. The name of the command comes from the T-splitter in plumbing, which has a shape like a lowercase "t".

The basic syntax of the command is:

```
command | tee file1 file2 ...
```

where "command" is the shell command to produce output, and "file1", "file2", etc. are the names of the files to write the output to. If a file with the specified name already exists, it will be overwritten. If a file does not exist, it will be created.

Another way to use the command is by using the "-a" option which will append the output to the specified file, rather than overwriting it. For example:

```
command | tee -a file1 file2 ...
```

In addition to writing to files, the "tee" command can also be used to display output on the screen and write it to a file at the same time. For example:

```
command | tee file1
```

will display the output on the screen and save it to file1.

Overall, "tee" can be useful when troubleshooting or debugging scripts, as it can be used to capture and analyze output from multiple stages of a pipeline or application. 

## tldr 
 
> Read from standard input and write to standard output and files (or commands).
> More information: <https://www.gnu.org/software/coreutils/tee>.

- Copy standard input to each file, and also to standard output:

`echo "example" | tee {{path/to/file}}`

- Append to the given files, do not overwrite:

`echo "example" | tee -a {{path/to/file}}`

- Print standard input to the terminal, and also pipe it into another program for further processing:

`echo "example" | tee {{/dev/tty}} | {{xargs printf "[%s]"}}`

- Create a directory called "example", count the number of characters in "example" and write "example" to the terminal:

`echo "example" | tee >(xargs mkdir) >(wc -c)`
