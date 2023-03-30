# while 
## chatgpt 
The `while` command is a programming construct that allows a specific block of code to be executed repeatedly as long as a certain condition is true. 

Here is the general syntax of a `while` loop:

```
while (condition) {
   // code to be executed repeatedly
}
```

The `condition` is a boolean expression that is evaluated before each iteration of the loop. If the condition is true, the block of code inside the `while` loop is executed. Once the code is finished executing, the condition is checked again, and the loop will continue to execute as long as the condition remains true.

A key feature of the `while` command is that it allows for indefinite looping, which means that the loop can run for an arbitrary number of iterations until a certain condition is met. To prevent infinite looping, it is important to make sure that the `condition` eventually becomes false. 

Here is a simple example of a `while` loop in Python:

```
x = 1
while x <= 5:
    print(x)
    x += 1
```

In this example, the `condition` is whether `x` is less than or equal to 5. Initially, `x` is set to 1, so the condition is true and the code inside the loop is executed. The `print()` function is called with the value of `x`, which is printed to the console. Then, `x` is incremented by 1 using the `+=` operator. 

The loop will repeat as long as the condition remains true, which means that `x` will be printed to the console in ascending order from 1 to 5. Once `x` becomes 6, the condition will evaluate to false, and the loop will terminate. 

Overall, the `while` command provides a flexible and powerful tool for creating iterative programs that can run for various durations and adapt to changing conditions. 

## tldr 
 
> Simple shell loop.
> More information: <https://manned.org/while>.

- Read `stdin` and perform an action on every line:

`while read line; do echo "$line"; done`

- Execute a command forever once every second:

`while :; do {{command}}; sleep 1; done`
