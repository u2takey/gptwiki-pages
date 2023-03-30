# xtrlock 
## chatgpt 
xtrlock is a command in Linux and Unix operating systems that locks an X display until a password is provided. When xtrlock is executed, it creates a window that covers the entire screen, making it impossible to access and use any applications or files on the desktop unless the correct password is entered.

To use xtrlock, the user must open a terminal window and type "xtrlock" followed by the Enter key. The screen will then be locked and will display a message prompting the user to enter the password.

The xtrlock command has several options that can be used to customize its behavior, such as specifying the font and size of the password prompt, setting the timeout for automatic lock, and enabling or disabling "mouse lock" to prevent movement of the mouse cursor while the screen is locked. 

Overall, xtrlock is a useful command for anyone who wants to secure their computer or prevent unauthorized access to their desktop. 

## tldr 
 
> Lock the X display until the user supplies their password.
> More information: <https://manned.org/xtrlock>.

- Lock the display and show a padlock instead of the cursor:

`xtrlock`

- Display a blank screen as well as the padlock cursor:

`xtrlock -b`

- Fork the xtrlock process and return immediately:

`xtrlock -f`
