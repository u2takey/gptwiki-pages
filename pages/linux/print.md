# print 
## chatgpt 
In general, "print" is a command that is commonly used in programming to output text or values to the console or screen.

In Python, the "print" command is a built-in function that allows you to display output to the console. The syntax of the "print" command is fairly straightforward - the command is written in lowercase letters followed by parentheses, and the data you want to output is enclosed within the parentheses, usually with quotation marks if it is a string.

Here's an example of how the "print" command can be used in Python:

```
print("Hello, world!")
```

In this case, the text "Hello, world!" will be displayed on the console.

You can also use the "print" command to output variables and expressions. For example:

```
x = 5
y = 10
print(x + y)
```

In this case, the value of x + y (which is 15) will be displayed on the console.

There are also a few additional options you can use with the "print" command, such as specifying how the output should be formatted using string formatting syntax, or using the "end" parameter to change the default newline character. 

## tldr 
 
> An alias to a `run-mailcap`'s action print.
> Originally `run-mailcap` is used to process mime-type/file.
> More information: <https://manned.org/print>.

- Print action can be used to print any file on default run-mailcap tool:

`print {{filename}}`

- With `run-mailcap`:

`run-mailcap --action=print {{filename}}`
