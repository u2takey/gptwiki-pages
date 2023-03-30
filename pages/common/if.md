# if 
## chatgpt 
The "if" command is a conditional statement used in various programming languages and in command-line interfaces. Its purpose is to control the execution of a block of code based on a specified condition or expression. 

In general, an "if" statement has the following structure:

if (condition) {
   // block of code to be executed if the condition is true
}

The condition is an expression that evaluates to either true or false. If it is true, the block of code inside the curly braces will be executed. If it is false, the block of code will be skipped and execution will continue with the next statement.

The "if" command is often used in conjunction with other conditional statements, such as "else" and "elseif", to provide more complex logic. For example:

if (condition1) {
   // block of code to be executed if condition1 is true
}
elseif (condition2) {
   // block of code to be executed if condition1 is false and condition2 is true
}
else {
   // block of code to be executed if both condition1 and condition2 are false
}

In summary, the "if" command allows programmers to control the flow of execution in their code based on specific conditions or expressions. 

## tldr 
 
> Performs conditional processing in shell scripts.
> See also: `test`, `[`.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#Conditional-Constructs>.

- Execute the specified commands if the condition command's exit status is zero:

`if {{condition_command}}; then {{echo "Condition is true"}}; fi`

- Execute the specified commands if the condition command's exit status is not zero:

`if ! {{condition_command}}; then {{echo "Condition is true"}}; fi`

- Execute the first specified commands if the condition command's exit status is zero otherwise execute the second specified commands:

`if {{condition_command}}; then {{echo "Condition is true"}}; else {{echo "Condition is false"}}; fi`

- Check whether a [f]ile exists:

`if [[ -f {{path/to/file}} ]]; then {{echo "Condition is true"}}; fi`

- Check whether a [d]irectory exists:

`if [[ -d {{path/to/directory}} ]]; then {{echo "Condition is true"}}; fi`

- Check whether a file or directory [e]xists:

`if [[ -e {{path/to/file_or_directory}} ]]; then {{echo "Condition is true"}}; fi`

- Check whether a variable is defined:

`if [[ -n "${{variable}}" ]]; then {{echo "Condition is true"}}; fi`

- List all possible conditions (`test` is an alias to `[`; both are commonly used with `if`):

`man [`
