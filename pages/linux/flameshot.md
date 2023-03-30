# flameshot 
## chatgpt 
Flameshot is a command-line tool that allows users to capture screenshots on their Linux systems. It is a powerful and flexible screenshot tool that lets users take screenshots of full screens, specific windows, or custom areas on their display.

Here is a detailed explanation of the Flameshot command and its most commonly used options:

- flameshot gui: This command launches the Flameshot Graphical User Interface (GUI), which allows users to take screenshots using a point-and-click interface.

- flameshot full: This command captures a screenshot of the entire screen.

- flameshot screen: This command captures a screenshot of the specified screen.

- flameshot window: This command captures a screenshot of the currently active window.

- flameshot select: This command allows users to select a custom region on the screen to capture.

- flameshot config: This command opens the configuration file for Flameshot, allowing users to customize the tool's behavior.

- flameshot save /PATH/TO/FILENAME.png: This command saves the captured screenshot with the specified filename and location.

Overall, Flameshot is a great tool for anyone who needs to take screenshots on a Linux system. Its flexible options and customizable configuration make it a must-have for developers and power users. 

## tldr 
 
> Screenshot utility with a GUI.
> Supports basic image editing, such as text, shapes, colors, and imgur.
> More information: <https://flameshot.org>.

- Create a fullscreen screenshot:

`flameshot full`

- Create a screenshot interactively:

`flameshot gui`

- Create a screenshot and save it to a specific path:

`flameshot gui --path {{path/to/directory}}`

- Create a screenshot interactively in a simplified mode:

`flameshot launcher`

- Create a screenshot from a specific monitor:

`flameshot screen --number {{2}}`

- Create a screenshot and print it to the standard output:

`flameshot gui --raw`

- Create a screenshot and copy it to the clipboard:

`flameshot gui --clipboard`

- Create a screenshot with a specific delay in milliseconds:

`flameshot full --delay {{5000}}`
