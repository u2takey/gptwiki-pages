# read 
## chatgpt 
The "read" command is used to take input from the user or a file and store it in a variable. It pauses the shell script and waits for the user to input data, which is assigned to the specified variable. The input can be a string, a number, or any other data type. 

The syntax for using the read command is as follows: 

```
read [options] variable_name
```

Here, "variable_name" is the name of the variable in which the input will be stored. The read command waits for the input from the user or file, and then stores it in the variable.

Some of the options that can be used with the read command are:

- -p: It provides a prompt for the user to enter the input.
- -r: It disables the interpretation of the backslash character.
- -t: It specifies the timeout interval for the input.

For example, the following command reads the user input and stores it in the variable "name":

```bash
read -p "Please enter your name: " name
```

After entering the input, the variable "name" will contain the value entered by the user. 

## tldr 
 
> BASH builtin for retrieving data from standard input.
> More information: <https://manned.org/read.1p>.

- Store data that you type from the keyboard:

`read {{variable}}`

- Store each of the next lines you enter as values of an array:

`read -a {{array}}`

- Specify the number of maximum characters to be read:

`read -n {{character_count}} {{variable}}`

- Use a specific character as a delimiter instead of a new line:

`read -d {{new_delimiter}} {{variable}}`

- Do not let backslash (\\) act as an escape character:

`read -r {{variable}}`

- Display a prompt before the input:

`read -p "{{Enter your input here: }}" {{variable}}`

- Do not echo typed characters (silent mode):

`read -s {{variable}}`

- Read `stdin` and perform an action on every line:

`while read line; do echo "$line"; done`
