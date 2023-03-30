# adb logcat 
## chatgpt 
The "adb logcat" command is used in Android Debug Bridge (ADB) to view system logs on an Android device. "ADB" is a command-line tool that allows a developer to communicate with an Android device connected through a USB cable or wirelessly using Wi-Fi. "Logcat" is a command in the ADB that retrieves and displays the system logs of an Android device.

The logcat command provides real-time output of the device's system logs, which are categorized into error, warning, info, and debug levels. These logs contain valuable information about system performance, application usage, and debugging information.

When executed, the adb logcat command shows the system logs outputted to the console/logcat window, and continuously updates as new logs are generated. This makes it a useful tool for developers to debug their applications and diagnose any issues on an Android device. Additionally, the logcat command can be filtered by specified tags or keywords to focus on specific logs of interest. 

Overall, the adb logcat command is an essential tool for Android developers and administrators to monitor and debug the system logs of an Android device. 

## tldr 
 
> Dump a log of system messages.
> More information: <https://developer.android.com/studio/command-line/logcat>.

- Display system logs:

`adb logcat`

- Display lines that match a regular expression:

`adb logcat -e {{regular_expression}}`

- Display logs for a tag in a specific mode ([V]erbose, [D]ebug, [I]nfo, [W]arning, [E]rror, [F]atal, [S]ilent), filtering other tags:

`adb logcat {{tag}}:{{mode}} *:S`

- Display logs for React Native applications in [V]erbose mode [S]ilencing other tags:

`adb logcat ReactNative:V ReactNativeJS:V *:S`

- Display logs for all tags with priority level [W]arning and higher:

`adb logcat *:W`

- Color the log (usually use with filters):

`adb logcat -v color`
