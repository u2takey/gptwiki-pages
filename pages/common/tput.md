# tput 
## chatgpt 
The command "tput" is a terminal utility command used to set or query terminal characteristics, such as cursor movement, color, and screen capabilities. It is commonly used in shell scripts and terminal applications to enable dynamic user interfaces and perform terminal manipulations.

The "tput" command typically takes one of two forms: "tput set" or "tput get". The "tput set" commands are used to set various terminal properties, such as cursor position or screen color. The "tput get" commands are used to retrieve information about the terminal, such as its size, capabilities, or current color settings.

Some common examples of "tput set" commands include:

- tput cup row col - moves the cursor to the specified row and column position
- tput setaf color - sets the text color to the specified color number
- tput setab color - sets the background color to the specified color number
- tput smso - enables standout mode (reverse video)

Some common examples of "tput get" commands include:

- tput lines - retrieves the number of lines in the terminal window
- tput cols - retrieves the number of columns in the terminal window
- tput colors - retrieves the number of colors supported by the terminal

In summary, the "tput" command is a versatile tool for performing terminal manipulations and retrieving information about the terminal environment. Its usage varies depending on the specific application or use case. 

## tldr 
 
> View and modify terminal settings and capabilities.
> More information: <https://manned.org/tput>.

- Move the cursor to a screen location:

`tput cup {{row}} {{column}}`

- Set foreground (af) or background (ab) color:

`tput {{setaf|setab}} {{ansi_color_code}}`

- Show number of columns, lines, or colors:

`tput {{cols|lines|colors}}`

- Ring the terminal bell:

`tput bel`

- Reset all terminal attributes:

`tput sgr0`

- Enable or disable word wrap:

`tput {{smam|rmam}}`
