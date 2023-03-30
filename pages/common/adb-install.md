# adb install 
## chatgpt 
adb install is a command used in Android Debug Bridge (ADB) tool to install an application package (.apk) onto an Android device connected to a computer. 

The syntax for the command is: 

adb install [options] package_path

Here, 'options' refer to additional parameters that can be used with the command, and 'package_path' is the path to the .apk file that needs to be installed. 

When this command is executed, the ADB tool transfers the .apk file from the computer to the Android device and installs it on the device. The installation process can be monitored in the device's notifications panel, which displays the progress of the installation.

Some common options that can be used with the adb install command are:

-s : Installs the application on the device's external storage (if available)
-r : Replaces an existing application with the same package name

It is important to note that in order to use the adb install command, USB debugging must be enabled on the Android device, and the ADB tool must be installed on the computer. 

## tldr 
 
> Android Debug Bridge Install: Push packages to an Android emulator instance or connected Android devices.
> More information: <https://developer.android.com/studio/command-line/adb>.

- Push an Android application to an emulator/device:

`adb install {{path/to/file.apk}}`

- Push an Android application to a specific emulator/device (overrides `$ANDROID_SERIAL`):

`adb -s {{serial_number}} install {{path/to/file.apk}}`

- Reinstall an existing app, keeping its data:

`adb install -r {{path/to/file.apk}}`

- Push an Android application allowing version code downgrade (debuggable packages only):

`adb install -d {{path/to/file.apk}}`

- Grant all permissions listed in the app manifest:

`adb install -g {{path/to/file.apk}}`

- Quickly update an installed package by only updating the parts of the APK that changed:

`adb install --fastdeploy {{path/to/file.apk}}`
