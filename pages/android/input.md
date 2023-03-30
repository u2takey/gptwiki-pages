# input 
## chatgpt 
The "input" command in computer programming is used to ask for user input. It prompts the user to type in some information, which can then be used by the program in various ways, such as performing calculations or making decisions. 

In Python, the "input" command is used to collect user input in the form of a string. For example:

```
name = input("What is your name? ")
```

This code will display the message "What is your name?" to the user and wait for them to enter their name. Whatever the user types in will be stored as a string in the "name" variable. 

It's important to note that the "input" command only collects data as a string, so if you need to perform calculations or comparisons with the inputted data, you may need to convert it to a different data type (such as an integer or float) using type conversion functions like int() or float(). 

## tldr 
 
> Send event codes or touchscreen gestures to an Android device.
> This command can only be used through `adb shell`.
> More information: <https://developer.android.com/reference/android/view/KeyEvent.html#constants_1>.

- Send an event code for a single character to an Android device:

`input keyevent {{event_code}}`

- Send a text to an Android device (`%s` represents spaces):

`input text "{{text}}"`

- Send a single tap to an Android device:

`input tap {{x_position}} {{y_position}}`

- Send a swipe gesture to an Android device:

`input swipe {{x_start}} {{y_start}} {{x_end}} {{y_end}} {{duration_in_ms}}`

- Send a long press to an Android device using a swipe gesture:

`input swipe {{x_position}} {{y_position}} {{x_position}} {{y_position}} {{duration_in_ms}}`
