# typeset 
## chatgpt 
The `typeset` command is used in Unix and Linux operating systems to declare variables and set their attributes. It allows the user to define the type of the variable, restrict its value to a specific range or set of values, and specify its scope (local or global).

The syntax for the `typeset` command is as follows:

```
typeset [option] variable=value
```

Here, `option` is used to set attributes such as the variable type (`-i` for integer, `-r` for read-only), the variable scope (`-g` for global), and so on. `variable` is the name of the variable to be declared, and `value` is its initial value.

For example, the following command declares a local integer variable named `count` and sets its initial value to 0:

```
typeset -i count=0
```

The `typeset` command can also be used to set attributes for existing variables, without changing their value. For instance, the following command sets the `LANG` environment variable to `en_US.utf8`:

```
typeset -x LANG=en_US.utf8
```

In summary, the `typeset` command is a powerful tool for declaring and defining variables in Unix and Linux systems, as it allows the user to set various attributes and restrictions on their use. 

## tldr 
 
> Declare variables and give them attributes.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#Bash-Builtins>.

- Declare a string variable with the specified value:

`typeset {{variable}}="{{value}}"`

- Declare an integer variable with the specified value:

`typeset -i {{variable}}="{{value}}"`

- Declare an array variable with the specified value:

`typeset {{variable}}=({{item_a item_b item_c}})`

- Declare an associative array variable with the specified value:

`typeset -A {{variable}}=({{[key_a]=item_a [key_b]=item_b [key_c]=item_c}})`

- Declare a readonly variable with the specified value:

`typeset -r {{variable}}="{{value}}"`

- Declare a global variable within a function with the specified value:

`typeset -g {{variable}}="{{value}}"`
