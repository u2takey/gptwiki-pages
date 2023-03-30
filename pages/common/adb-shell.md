# adb shell 
## chatgpt 
`adb shell` is a command that is used to open a shell in the Android Debug Bridge (ADB) on a connected Android device. This command can be used to access the device's file system, run shell commands on the device, debug applications, and more.

Here's a detailed explanation of what each part of the command does:

- `adb`: stands for Android Debug Bridge, a command-line tool used for communicating with Android devices.
- `shell`: is an argument that tells ADB to open a shell session on the device. A shell is essentially a command-line interface that allows users to interact with the device's operating system directly.

When you run `adb shell`, you'll be able to execute commands on the connected device in the same way you would if you were typing them into a terminal on the device itself. 

Once the shell is open, you can use commands like `ls` to list files and directories on the device, `cd` to change directories, `rm` to delete files, and `mkdir` to create folders. You can also run any other shell commands, such as creating environment variables, executing scripts, or running system commands. 

## tldr 
 
> Android Debug Bridge Shell: Run remote shell commands on an Android emulator instance or connected Android devices.
> More information: <https://developer.android.com/studio/command-line/adb>.

- Start a remote interactive shell on the emulator or device:

`adb shell`

- Get all the properties from emulator or device:

`adb shell getprop`

- Revert all runtime permissions to their default:

`adb shell pm reset-permissions`

- Revoke a dangerous permission for an application:

`adb shell pm revoke {{package}} {{permission}}`

- Trigger a key event:

`adb shell input keyevent {{keycode}}`

- Clear the data of an application on an emulator or device:

`adb shell pm clear {{package}}`

- Start an activity on emulator or device:

`adb shell am start -n {{package}}/{{activity}}`

- Start the home activity on an emulator or device:

`adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN`
