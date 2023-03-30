# local 
## chatgpt 
The "local" command is used in shell scripts to declare a variable as local within a function. When a variable is declared as local, its scope is limited to the function within which it is defined, meaning that any changes made to the variable within the function will not affect its value outside of the function.

When the "local" command is used, it is followed by the name of the variable(s) that is being declared as local. For example:

```
function myFunction {
  local myVariable=10
  # do something with myVariable
}
```

In this example, the "local" command is used to declare a variable called "myVariable" within the "myFunction" function. This means that "myVariable" cannot be accessed outside of the function, and any changes made to it within the function will not affect its value outside of the function.

Using the "local" command can be useful in larger scripts where multiple functions may be using the same variable names, as it ensures that any changes made to a variable within a function will not affect the value of the same variable used in another function. It also helps to prevent accidentally overwriting global variables within a function. 

## tldr 
 
> Declare local variables and give them attributes.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#Bash-Builtins>.

- Declare a string variable with the specified value:

`local {{variable}}="{{value}}"`

- Declare an integer variable with the specified value:

`local -i {{variable}}="{{value}}"`

- Declare an array variable with the specified value:

`local {{variable}}=({{item_a item_b item_c}})`

- Declare an associative array variable with the specified value:

`local -A {{variable}}=({{[key_a]=item_a [key_b]=item_b [key_c]=item_c}})`

- Declare a readonly variable with the specified value:

`local -r {{variable}}="{{value}}"`
