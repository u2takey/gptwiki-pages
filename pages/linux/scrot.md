# scrot 
## chatgpt 
scrot is a Linux command-line tool used to capture screenshots of the desktop. The command is used to take a screenshot of the full desktop or a portion of the screen. Here is the syntax of the command:

` scrot [options] [file_name]`

- Options: These are additional arguments passed to the command to modify the behavior of the screenshot. Different options can be used to specify the type of screenshot to take, the format of the output file, the delay before capturing the screenshot, among others.

- file_name: This is the name of the output file where the screenshot will be saved. This argument is optional, and if not specified, the screenshot will be saved in the current working directory with a default name.

Some of the common options used with scrot command are:

- `-s`: This option allows you to capture a portion of the screen by selecting a rectangular area to screenshot.

- `-d [seconds]`: This option adds a delay before taking the screenshot, allowing the user to set up the screen beforehand.

- `--quality [percentage]`: This option sets the quality of the captured screenshot in percentage.

- `-h`: This option provides the help guide for the command with brief instructions.

Overall, the scrot command is useful for capturing screenshots in a simple and convenient way on Linux command-line systems. 

## tldr 
 
> Screen capture utility.
> More information: <https://github.com/resurrecting-open-source-projects/scrot>.

- Capture a screenshot and save it to the current directory with the current date as the filename:

`scrot`

- Capture a screenshot and save it as `capture.png`:

`scrot {{capture.png}}`

- Capture a screenshot interactively:

`scrot --select`

- Capture a screenshot from the currently focused window:

`scrot --focused`

- Display a countdown of 10 seconds before taking a screenshot:

`scrot --count --delay {{10}}`
