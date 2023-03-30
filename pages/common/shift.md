# shift 
## chatgpt 
The `shift` command is a built-in command in Unix-based operating systems, including Linux and macOS. It is used to shift the positional parameters passed to a shell script or function to the left by a specified number of positions. 

The syntax of the `shift` command is as follows:

```
shift [n]
```

Here, `n` is an optional parameter that specifies how many positions to shift the positional parameters. If `n` is not provided, the default value is 1, meaning that the first positional parameter is removed and all others are shifted to the left.

The `shift` command is typically used in shell scripts or functions to process command-line arguments. For example, consider the following shell script that takes three arguments and uses them to print a message:

```
#!/bin/bash

echo "Hello, $1 $2 $3!"
```

If this script is called with the command `./greeting.sh Alice Bob Carol`, it will output:

```
Hello, Alice Bob Carol!
```

However, if we want to use the positional parameters in a different order, we can use the `shift` command to move them around. For example, suppose we want to print the message with the first and third parameters swapped:

```
#!/bin/bash

shift
echo "Hello, $2 $1 $3!"
```

With this updated script, the command `./greeting.sh Alice Bob Carol` will output:

```
Hello, Bob Alice Carol!
```

The `shift` command removes the first positional parameter (i.e., `Alice`), so `$2` now refers to `Bob`, and `$1` refers to `Carol`. Note that when using the `shift` command, the position of the parameters in the script changes, so subsequent references to them must be adjusted accordingly. 

## tldr 
 
> Bash built-in command that shifts the arguments passed to the calling function or script by a specified number of places.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#index-shift>.

- Move arguments by one place dropping the first argument:

`shift`

- Move arguments by N places dropping the first N arguments:

`shift {{N}}`
