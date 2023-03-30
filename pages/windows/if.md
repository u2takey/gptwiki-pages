# if 
## chatgpt 
The "if" command is a conditional statement used in programming languages and operating systems. It allows the program to execute specific actions based on whether a defined condition is true or false.

Here are the main components of the "if" command:

1. Condition: This is the statement that determines whether the condition is true or false.

2. Action: This is the action that will be executed if the condition is true.

3. Else: If the condition is false, the action in the else block will be executed.

The syntax of the "if" command varies depending on the programming language or operating system you are using. However, the general structure is as follows:

if (condition) {

action if true;

} else {

action if false;

}

For example, in Python:

if x > 10:
  print("x is greater than 10")
else:
  print("x is less than or equal to 10")

In this example, the condition is "x > 10", and the action if true is "print('x is greater than 10')". If the condition is false, the action in the else block will be executed, which is "print('x is less than or equal to 10')".

In summary, the "if" command is a conditional statement that allows for decision-making within a program based on the truth of a condition. 

## tldr 
 
> Performs conditional processing in batch scripts.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/if>.

- Execute the specified commands if the condition is true:

`if {{condition}} ({{echo Condition is true}})`

- Execute the specified commands if the condition is false:

`if not {{condition}} ({{echo Condition is true}})`

- Execute the first specified commands if the condition is true otherwise execute the second specified commands:

`if {{condition}} ({{echo Condition is true}}) else ({{echo Condition is false}})`

- Check whether `%errorlevel%` is greater than or equal to the specified exit code:

`if errorlevel {{2}} ({{echo Condition is true}})`

- Check whether two strings are equal:

`if %{{variable}}% == {{string}} ({{echo Condition is true}})`

- Check whether two strings are equal without respecting letter case:

`if /i %{{variable}}% == {{string}} ({{echo Condition is true}})`

- Check whether a file exist:

`if exist {{path\to\file}} ({{echo Condition is true}})`
