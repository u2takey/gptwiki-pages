# declare 
## chatgpt 
The `declare` command is a shell built-in command in Linux and Unix systems. It is used to declare variables, assign attributes to variables, define functions and update shell options. The `declare` command can be used to set the variable properties as string, integer or array types. 

The syntax of the declare command is:

```
declare [option] variable=value
```

Where `option` is an optional parameter that can be used to assign an attribute to the variable being declared. Some commonly used options are:

- `-a`: Declare the variable as an array.
- `-i`: Declare the variable as an integer.
- `-r`: Declare the variable as read-only.
- `-x`: Export the variable to be available to child processes.

The `value` parameter is optional and is used to initialize the variable with a value. If the `value` parameter is not specified, the variable will be initialized as an empty string.

Examples:

1. Declare and initialize a variable as an integer:

```
declare -i num=10
echo $num
```

Output: 
```
10
``` 

2. Declare and initialize an array variable:

```
declare -a arr=('apple' 'banana' 'orange')
echo ${arr[1]}
```

Output:
```
banana
```

3. Define and execute a function:

```
declare -f greet
function greet {
  echo "Hello, $1!"
}
greet "World"
```

Output:
```
Hello, World!
```

4. Declare a read-only variable:

```
declare -r readonly_var="This variable is read-only"
readonly_var="Can't modify this"
```

Output:
```
-bash: readonly_var: readonly variable
``` 

In summary, the `declare` command is used to define variables and functions with specified properties that can be used throughout the shell script. 

## tldr 
 
> Declare variables and give them attributes.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#Bash-Builtins>.

- Declare a string variable with the specified value:

`declare {{variable}}="{{value}}"`

- Declare an integer variable with the specified value:

`declare -i {{variable}}="{{value}}"`

- Declare an array variable with the specified value:

`declare -a {{variable}}=({{item_a item_b item_c}})`

- Declare an associative array variable with the specified value:

`declare -A {{variable}}=({{[key_a]=item_a [key_b]=item_b [key_c]=item_c}})`

- Declare a readonly string variable with the specified value:

`declare -r {{variable}}="{{value}}"`

- Declare a global variable within a function with the specified value:

`declare -g {{variable}}="{{value}}"`
