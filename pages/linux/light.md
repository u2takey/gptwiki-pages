# light 
## chatgpt 
I'm assuming you are referring to the Linux command "light". 

The "light" command is used to control the backlight brightness of the screen. 

Here's how you can use the "light" command:

1. Check if the "light" command is installed on your system by opening a terminal and executing "light --version". If it is not installed, you can install it using your package manager. 

2. To get the current brightness value, execute "light -G". It will return a value between 0 and 100. 

3. To set the brightness to a specific value, execute "light -S VALUE", where VALUE is the desired brightness level between 0 and 100. 

4. You can also increment or decrement the brightness with the "+VALUE" or "-VALUE" option. 

Overall, the "light" command can be useful for conserving battery life on laptops or adjusting screen brightness to your personal preference. 

## tldr 
 
> CLI to control the backlight of your screen.
> More information: <https://manned.org/light>.

- Get the current backlight value in percent:

`light`

- Set the backlight value to 50 percent:

`light -S {{50}}`

- Reduce 20 percent from the current backlight value:

`light -U {{20}}`

- Add 20 percent to the current backlight value:

`light -A {{20}}`
