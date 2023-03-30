# emulator 
## chatgpt 
The emulator command is a command-line tool that is part of the Android SDK, and it is used to run and manage Android virtual devices (AVDs). An AVD is a software-based emulation of an Android device, which allows developers to test their applications on different device configurations and versions of the Android operating system.

Here are some of the common options and parameters that can be used with the emulator command:

- `-avd <avd_name>`: Specifies the name of the AVD to run. If this option is omitted, the command will show a list of available AVDs.
- `-writable-system`: Allows modifications to system files on the virtual device. Without this option, the system files are read-only.
- `-no-boot-anim`: Disables the boot animation on the virtual device.
- `-no-snapshot-load`: Disables loading from a previously saved snapshot of the virtual device. This can be useful for testing the start-up performance of an app.
- `-gpu <mode>`: Specifies the mode of graphics acceleration to use on the virtual device. Possible values include "auto", "swiftshader", "angle_indirect", "angle_direct", and "guest".
- `-ports <console_port>,<adb_port>`: Specifies the ports to use for the emulator console and Android Debug Bridge (ADB) connections.

Overall, the emulator command is an essential tool for Android app development, as it allows developers to test their apps in a controlled and repeatable environment before deploying them to real devices. 

## tldr 
 
> Manager Android emulators from the command-line.
> More information: <https://developer.android.com/studio/run/emulator-commandline>.

- Display the help:

`emulator -help`

- Start an Android emulator device:

`emulator -avd {{name}}`

- Display the webcams on your development computer that are available for emulation:

`emulator -avd {{name}} -webcam-list`

- Start an emulator overriding the facing back camera setting (use `-camera-front` for front camera):

`emulator -avd {{name}} -camera-back {{none|emulated|webcamN}}`

- Start an emulator, with a maximum network speed:

`emulator -avd {{name}} -netspeed {{gsm|hscsd|gprs|edge|hsdpa|lte|evdo|full}}`

- Start an emulator with network latency:

`emulator -avd {{name}} -netdelay {{gsm|hscsd|gprs|edge|hsdpa|lte|evdo|none}}`

- Start an emulator, making all TCP connections through a specified HTTP/HTTPS proxy (port number is required):

`emulator -avd {{name}} -http-proxy {{http://example.com:80}}`

- Start an emulator with a given SD card partition image file:

`emulator -avd {{name}} -sdcard {{path/to/sdcard.img}}`
