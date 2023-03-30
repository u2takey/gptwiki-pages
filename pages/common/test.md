# test 
## chatgpt 
The `test` command is a built-in command in Linux and Unix systems used to evaluate expressions and return a Boolean value (true or false) based on whether the expression is true or false.

A typical syntax of the `test` command is as follows:

```
test expression
```

Here, `expression` is a condition or test that you want to evaluate. Depending on the type of expression used, the `test` command can evaluate various conditions such as file existence, file type, file permissions, string comparisons, numeric comparisons, and more.

For instance, if you want to check if a file exists in a directory, you can use the following command:

```
test -e /path/to/file
```

Here, `e` is a flag that stands for "exist", and `/path/to/file` is the path to the file you want to check. If the file exists, the `test` command returns true (0); otherwise, it returns false (1).

Similarly, you can check various conditions using different flags and expressions with the `test` command. You can also use the `[` command as an alias for `test`, like:

```
[ expression ]
```

Note that the `test` command is often used in shell scripts and in combination with other commands to create conditional statements and control flow operations. 

## tldr 
 
> Check file types and compare values.
> Returns 0 if the condition evaluates to true, 1 if it evaluates to false.
> More information: <https://www.gnu.org/software/coreutils/test>.

- Test if a given variable is equal to a given string:

`test "{{$MY_VAR}}" == "{{/bin/zsh}}"`

- Test if a given variable is empty:

`test -z "{{$GIT_BRANCH}}"`

- Test if a file exists:

`test -f "{{path/to/file_or_directory}}"`

- Test if a directory does not exist:

`test ! -d "{{path/to/directory}}"`

- If A is true, then do B, or C in the case of an error (notice that C may run even if A fails):

`test {{condition}} && {{echo "true"}} || {{echo "false"}}`
