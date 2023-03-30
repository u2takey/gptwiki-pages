# screencap 
## chatgpt 
The command "screencap" is a command used on Android devices to take a screenshot of the current screen view. When the command is executed, the device's screen is instantly captured as an image and saved in the device's designated screenshots folder. Here are some important points to know about using the "screencap" command:

- Syntax: screencap <filename.png> - This indicates that the command is followed by the name of the file that will be generated in PNG format.
- Root access: The device needs to be rooted to use the "screencap" command. If the device is not rooted, the command will fail.
- ADB connection: The device needs to be connected to a computer via ADB (Android Debug Bridge) to execute the "screencap" command. ADB is a command line tool that allows developers to interact with Android devices from a computer.
- File transfer: Once the file is captured, it needs to be transferred to the computer. This can be done using the ADB "pull" command.
- File location: The file will be saved in the "Pictures" folder on the device's internal storage unless specified otherwise.
- Additional parameters: The "screencap" command can also be followed by additional parameters such as the device ID (in case of multiple connected devices) and the file format.

Overall, the "screencap" command provides an easy way to take a screenshot of an Android device's screen without having to rely on third-party apps or hardware. 

## tldr 
 
> Take a screenshot of a mobile display.
> This command can only be used through `adb shell`.
> More information: <https://developer.android.com/studio/command-line/adb#screencap>.

- Take a screenshot:

`screencap {{path/to/file}}`
