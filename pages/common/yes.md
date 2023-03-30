# yes 
## chatgpt 
The "yes" command is a simple command that outputs an endless stream of "y" characters to the console until interrupted. It can be used for a variety of purposes such as testing and automation scripts, filling up disk space or buffers for stress testing, or even for trolling.

By default, running the "yes" command will continuously print the letter 'y' to the console. If you want to output a different character or string, you can use the following syntax: "yes [string]" where [string] is the character or string you want to output infinitely.

For example, you can use the following command to output the word "Hello" continuously:

yes "Hello"

To stop the output, you need to interrupt the process. You can do this by pressing Ctrl+C on your keyboard.

Overall, the "yes" command is a simple but powerful tool that can be used for a variety of purposes in different scenarios. 

## tldr 
 
> Output something repeatedly.
> This command is commonly used to answer yes to every prompt by install commands (such as apt-get).
> More information: <https://www.gnu.org/software/coreutils/yes>.

- Repeatedly output "message":

`yes {{message}}`

- Repeatedly output "y":

`yes`

- Accept everything prompted by the `apt-get` command:

`yes | sudo apt-get install {{program}}`
