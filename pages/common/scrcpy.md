# scrcpy 
## chatgpt 
scrcpy is a command-line tool used for displaying and controlling Android devices from a desktop computer. It allows users to mirror their Android device screen onto their computer and control it using the computer keyboard and mouse.

This tool requires the Android device to have adb (Android Debug Bridge) running in the background. The scrcpy software will use this connection and stream the video and audio from the Android device to the desktop computer. The video stream runs at a high frame rate, making it responsive and suitable for gaming or other interactive applications.

To use scrcpy, simply run the command “scrcpy” in a terminal or command prompt window after installation. The tool will detect the device connected to the computer and begin streaming the device screen to the computer.

Additional options can be specified on the command line to control the behavior of scrcpy. These include screen resolution, orientation, bit rate, cropping, and more. See the scrcpy documentation for more information. 

## tldr 
 
> Display and control your Android device on a desktop.
> More information: <https://github.com/Genymobile/scrcpy>.

- Display a mirror of a connected device:

`scrcpy`

- Display a mirror of a specific device based on its ID or IP address (find it under the `adb devices` command):

`scrcpy --serial {{0123456789abcdef|192.168.0.1:5555}}`

- Start display in fullscreen mode:

`scrcpy --fullscreen`

- Rotate the display screen. Each incremental value adds a 90 degree counterclockwise rotation:

`scrcpy --rotation {{0|1|2|3}}`

- Show touches on physical device:

`scrcpy --show-touches`

- Record display screen:

`scrcpy --record {{path/to/file.mp4}}`

- Set target directory for pushing files to device by drag and drop (non-APK):

`scrcpy --push-target {{path/to/directory}}`
