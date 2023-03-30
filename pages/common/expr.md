# expr 
## chatgpt 
The command "expr" is a utility found in Unix-based operating systems that allows you to evaluate expressions and perform mathematical operations in the command line. It accepts one or more arguments, which can be mathematical expressions or string manipulations.

The syntax for the "expr" command is as follows:

expr expression

The "expression" can include various operators such as addition, subtraction, multiplication, and division. For example, if you want to add two numbers, you can use the following command:

$ expr 2 + 3

This will output "5" as the result. Similarly, if you want to subtract two numbers, you can use the following command:

$ expr 5 - 3

This will output "2" as the result.

Apart from mathematical operations, the "expr" command can also be used for string manipulations, such as extracting substrings or finding the length of a string. For example, the following command extracts the substring "world" from the string "hello world":

$ expr "hello world" : '.*\(world\)'

The above command uses regular expressions to search for the pattern matching "world" and extracts it as a substring.

Overall, the "expr" command is useful for performing mathematical and string operations in shell scripts or in the command line. 

## tldr 
 
> Evaluate expressions and manipulate strings.
> More information: <https://www.gnu.org/software/coreutils/expr>.

- Get the length of a specific string:

`expr length "{{string}}"`

- Get the substring of a string with a specific length:

`expr substr "{{string}}" {{from}} {{length}}`

- Match a specific substring against an anchored pattern:

`expr match "{{string}}" '{{pattern}}'`

- Get the first char position from a specific set in a string:

`expr index "{{string}}" "{{chars}}"`

- Calculate a specific mathematic expression:

`expr {{expression1}} {{+|-|*|/|%}} {{expression2}}`

- Get the first expression if its value is non-zero and not null otherwise get the second one:

`expr {{expression1}} \| {{expression2}}`

- Get the first expression if both expressions are non-zero and not null otherwise get zero:

`expr {{expression1}} \& {{expression2}}`
