# print 
## chatgpt 
The "print" command is used in programming to display information or output on the console or terminal. It allows the developer to see the result of their code, which is essential for debugging and testing purposes. 

The syntax for the "print" command may vary depending on the programming language being used. However, in general, it involves passing a value or a list of values as an argument to the command, separated by commas or concatenation operators.

For example, in Python, the syntax for the "print" command is as follows:

```
print(value1, value2, ..., sep=' ', end='\n', file=sys.stdout, flush=False)
```

Here, "value1", "value2", etc. are the values we want to print on the console. The "sep" parameter is used to specify the separator between the values (by default, it is a space). The "end" parameter is used to specify what should be printed after the values (by default, it is a newline). The "file" parameter allows us to specify the output file to which the printed values will be written. Finally, the "flush" parameter is used to force the output to appear immediately, without buffering.

Overall, the "print" command is a very useful tool for developers to check their code and understand what is happening behind the scenes. 

## tldr 
 
> Print a text file to a printer.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/print>.

- Print a text file to the default printer:

`print {{path\to\file}}`

- Print a text file to a specific printer:

`print /d:{{printer}} {{path\to\file}}`
