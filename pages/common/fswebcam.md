# fswebcam 
## chatgpt 
fswebcam is a command-line utility used on Linux-based operating systems to capture images and videos from a webcam. 

Here's a breakdown of the command's syntax:

`fswebcam [OPTIONS] FILENAME`

- `fswebcam`: The name of the command itself. Invoking it will cause it to execute on the user's system. 
- `[OPTIONS]`: These are the available options or flags that can be passed to fswebcam. They can modify how the command behaves for a given capture session. 
- `FILENAME`: This is the name of the file where the captured image or video will be saved. It can be a full or relative path on the local file system. 

Some common options available with fswebcam include:

- `-r` or `--resolution`: This option sets the resolution of the captured image or video. It takes a value in the format `<width>x<height>`, e.g. `640x480`.
- `-S` or `--set`: This option allows users to manually adjust the camera settings, such as brightness or contrast. It takes a string of key-value pairs, separated by commas. 
- `-s` or `--save`: This option specifies the folder where the captured files should be saved. 
- `-l` or `--list-controls`: This option lists the camera controls that can be manually adjusted using the `-S` option. 
- `-h` or `--help`: This option prints a help message for the command. 

Overall, fswebcam is a useful command-line utility for quickly capturing images or videos from a webcam on Linux-based systems. 

## tldr 
 
> Small and simple webcam for *nix.
> More information: <https://www.sanslogic.co.uk/fswebcam>.

- Take a picture:

`fswebcam {{filename}}`

- Take a picture with custom resolution:

`fswebcam -r {{width}}x{{height}} {{filename}}`

- Take a picture from selected device(Default is `/dev/video0`):

`fswebcam -d {{device}} {{filename}}`

- Take a picture with timestamp(timestamp string is formatted by strftime):

`fswebcam --timestamp {{timestamp}} {{filename}}`
