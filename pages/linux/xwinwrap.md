# xwinwrap 
## chatgpt 
`xwinwrap` is an X Window System utility that allows you to run any program as the desktop background. It creates a window around the specified program and renders it on the desktop, giving the appearance of a moving background.

The command syntax for `xwinwrap` is:

```
xwinwrap [options] -g <geometry> -ni -s -nf -- <command> [args...]
```

Here is what each option means:

- `[options]`: Optional arguments that configure specific settings.
- `-g <geometry>`: Specifies the window size and position, using the standard X Window System geometry specification.
- `-ni`: Specifies that the created window should be marked as "not input", which means it will not accept any input events such as clicks or key presses.
- `-s`: Specifies that the created window should be parented to the root window, which allows it to be rendered on top of the desktop.
- `-nf`: Specifies that the created window should not have a focus indication, which means it will not respond to focus-related events.
- `--`: Separates the `xwinwrap` arguments from the command to be run in the background.
- `<command> [args...]`: Specifies the program to be run as the desktop background.

Here is an example of how to use `xwinwrap` to run a video as the desktop background:

```
xwinwrap -g 1920x1080+0+0 -ni -s -nf -- mpv -wid WID --no-audio /path/to/video.mp4
```

This starts `xwinwrap` with the following options:

- A geometry of 1920x1080 and position at (0, 0) (top-left corner of the screen).
- The window should be marked as "not input" and should not have a focus indication.
- The command to run in the background is `mpv -wid WID --no-audio /path/to/video.mp4`. This runs the `mpv` video player with the `--no-audio` flag (to prevent any audio output, since it's a desktop background) and specifies the `-wid` option to use the window ID created by `xwinwrap` as the target display for the video.

This will create a window with the specified size and position that plays the specified video as the desktop background, effectively replacing the static background image. 

## tldr 
 
> Run a player or a program as desktop background.
> More information: <https://github.com/ujjwal96/xwinwrap>.

- Run a video using mpv:

`xwinwrap -b -nf -ov -- {{mpv}} -wid {{wid}} --loop --no-audio --no-resume-playback --panscan={{1.0}} {{path/to/video.mp4}}`

- Run a video in fullscreen using mpv:

`xwinwrap -b -nf -fs -ov -- {{mpv}} -wid {{wid}} --loop --no-audio --no-resume-playback --panscan={{1.0}} {{path/to/video.mp4}}`

- Run a video using mpv with 80% opacity:

`xwinwrap -b -nf -ov -o 0.8 --- {{mpv}} -wid {{wid}} --loop --no-audio --no-resume-playback --panscan={{1.0}} {{path/to/video.mp4}}`

- Run a video using mpv in a second monitor 1600x900 with 1920 offset on X-axis:

`xwinwrap -g 1600x900+1920 -b -nf -ov -- {{mpv}} -wid {{wid}} --loop --no-audio --no-resume-playback --panscan={{1.0}} {{path/to/video.mkv}}`
