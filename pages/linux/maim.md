# maim 
## chatgpt 
The `maim` command is a Linux utility used to take screenshots of a particular area of the screen or the entire screen. Here is the detailed explanation of the command:

Syntax:
```
maim [OPTIONS]... [FILENAME]
```

Options:
- `-h`, `--help`: show help message and exit
- `-v`, `--version`: show version and exit
- `-c`, `--color`: save screenshot in color (default is grayscale)
- `-g`, `--geometry`: set geometry of the screenshot in the format `WxH+X+Y`, where `W` is the width, `H` is the height, `X` is the X-offset, and `Y` is the Y-offset
- `-s`, `--select`: start a selection window to choose the area to be screenshotted
- `-i`, `--window`: screenshot only the active window
- `-d`, `--delay`: add a delay (in seconds) before taking the screenshot
- `-m`, `--monitor`: screenshot a specific monitor (if multiple monitors are connected)
- `-u`, `--underline`: draw an underline under the mouse cursor in the screenshot
- `-b`, `--border`: draw a border around the screenshot
- `-p`, `--pointer`: include the mouse pointer in the screenshot
- `-l`, `--line`: draw a line from the top of the screenshot to the bottom
- `-f`, `--format`: set the output format (e.g. png, jpg)
- `-o`, `--open`: automatically open the screenshot with the default viewer

Examples:
1. Take a screenshot of the entire screen and save it as `screenshot.png`:
```
maim screenshot.png
```
2. Take a screenshot of a specific area of the screen and save it as `screenshot.png`:
```
maim -g 800x600+0+0 screenshot.png
```
3. Take a screenshot of the active window and save it as `screenshot.jpg`:
```
maim -i -f jpg screenshot.jpg
```
4. Take a screenshot of a specific monitor and save it as `screenshot.png`:
```
maim -m 1 screenshot.png
```
5. Start a selection window to choose the area to be screenshotted and save it as `screenshot.png`:
```
maim -s screenshot.png
``` 

## tldr 
 
> Screenshot utility.
> More information: <https://github.com/naelstrof/maim>.

- Capture a screenshot and save it to the given path:

`maim {{path/to/screenshot.png}}`

- Capture a screenshot of the selected region:

`maim --select {{path/to/screenshot.png}}`

- Capture a screenshot of the selected region and save it in the clipboard (requires `xclip`):

`maim --select | xclip -selection clipboard -target image/png`

- Capture a screenshot of the current active window (requires `xdotool`):

`maim --window $(xdotool getactivewindow) {{path/to/screenshot.png}}`
