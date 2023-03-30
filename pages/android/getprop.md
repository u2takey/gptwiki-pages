# getprop 
## chatgpt 
getprop is a command used in Android operating systems to retrieve system properties. System properties are stored as key-value pairs, and the getprop command is used to get the value of a specific property by specifying its key.

The getprop command is typically used in terminal or command-line interfaces on Android devices. Here is an example of how to use the getprop command:

1. Open a terminal or command prompt on your Android device.
2. Type "getprop" followed by the key of the property you want to retrieve. For example, to retrieve the value of the "ro.build.version.sdk" property (which represents the version of the Android SDK used to build the system image), you would type:

getprop ro.build.version.sdk

3. Press "Enter" to execute the command. The value of the specified property will be displayed in the terminal output.

The getprop command can be used to retrieve a wide range of system properties, including device information, system settings, and runtime environment variables. These properties can be useful for diagnosing problems with your device, developing apps that interact with system features, or customizing your Android experience. 

## tldr 
 
> Show information about Android system properties.
> More information: <https://manned.org/getprop>.

- Display information about Android system properties:

`getprop`

- Display information about a specific property:

`getprop {{property}}`

- Display the SDK API level:

`getprop {{ro.build.version.sdk}}`

- Display the Android version:

`getprop {{ro.build.version.release}}`

- Display the Android device model:

`getprop {{ro.vendor.product.model}}`

- Display the OEM unlock status:

`getprop {{ro.oem_unlock_supported}}`

- Display the MAC address of the Android's Wi-Fi card:

`getprop {{ro.boot.wifimacaddr}}`
