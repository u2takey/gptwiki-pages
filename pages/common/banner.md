# banner 
## chatgpt 
The banner command is a simple command used for printing banner characters in different styles on the terminal screen. The banner command takes a message as input and displays it in large and colorful letters using ASCII art.

Syntax:
banner [options] <message>

Options:
-w <width>: Specifies the width of the banner in characters. By default, the banner is printed in the full width of the terminal window.
-f <font>: Specifies the font style of the banner characters.
-a: Centers the banner message horizontally in the middle of the screen.
-n: Disables the automatic newline at the end of the output.

Example:
To print a banner message "Hello World" in a width of 20 characters and with the font style "big":
```
banner -w 20 -f big "Hello World"
```
Output:
```
  _  _  ____  __    ___   __   _  _ 
 ( \/ )(  _ \(  )  / __) / _\ ( \/ )
  \  /  )   / )(__( (__ /    \/ \/ \
  (__)(__/\\\_)\___)\___)\_/\_/\_)(_/
```
Note: The output may vary depending on the font style and screen dimensions. 

## tldr 
 
> Print the given argument as a large ASCII art.
> More information: <https://manned.org/banner>.

- Print the text message as a large banner (quotes are optional):

`banner "{{Hello World}}"`

- Print the text message as a banner with a width of 50 characters:

`banner -w {{50}} "{{Hello World}}"`

- Read text from `stdin`:

`banner`
