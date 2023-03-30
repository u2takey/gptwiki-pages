# urxvt 
## chatgpt 
`urxvt` (abbreviation of "​Rxvt unicode terminal emulator") is a lightweight terminal emulator for X Window System based on the popular Rxvt terminal emulator. It primarily provides features such as transparency, xft font support, Unicode character encoding, and more.

When the `urxvt` command is executed, it launches the terminal emulator, providing the user with an interface to execute various commands, interact with applications, and manage system resources. The emulator supports a range of customizable options including font, color, size, background, and more, allowing users to customize the terminal environment as per their personal preferences.

Some examples of command-line options that can be passed while invoking `urxvt` are:

- `-fn` - specifies the font name
- `-fb` - specifies the font size in pixels
- `-fg` - specifies the forecolor of text
- `-bg` - specifies the background color
- `-tr` - enables transparency
- `-tint` - sets a tint color for a transparent window
- `-e` - specifies the command to be executed in the terminal

Overall, `urxvt` is a simple and efficient terminal emulator that provides powerful features for developers, system administrators, and everyday users alike. 

## tldr 
 
> Rxvt-unicode.
> A customizable terminal emulator.
> More information: <https://manned.org/urxvt>.

- Open a new urxvt window:

`urxvt`

- Run in a specific directory:

`urxvt -cd {{path/to/directory}}`

- Run a command in a new urxvt window:

`urxvt -e {{command}}`

- Run a command and keep the window open:

`urxvt --hold -e {{command}}`

- Run a command within the `sh` shell:

`urxvt -e {{sh}} -c {{command}}`
