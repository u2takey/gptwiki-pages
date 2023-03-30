# pm 
## chatgpt 
The "pm" command is used in Android operating systems to manage app packages and their permissions. It requires root access or the "android.permission.PACKAGE_USAGE_STATS" permission to execute.

Here are some examples of how to use the "pm" command:

1. To list all installed packages on the device, use the command: "pm list packages"

2. To get information about a specific package, use the command: "pm dump PACKAGE_NAME"

3. To freeze or disable an app, use the command: "pm disable PACKAGE_NAME"

4. To enable a previously disabled app, use the command: "pm enable PACKAGE_NAME"

5. To grant a specific permission to an app, use the command: "pm grant PACKAGE_NAME android.permission.PERMISSION_NAME"

6. To revoke a specific permission from an app, use the command: "pm revoke PACKAGE_NAME android.permission.PERMISSION_NAME"

Overall, the "pm" command provides a powerful tool for managing app permissions and packages on Android devices. 

## tldr 
 
> Display information about apps on an Android device.
> More information: <https://developer.android.com/studio/command-line/adb#pm>.

- List all installed apps:

`pm list packages`

- List all installed system apps:

`pm list packages -s`

- List all installed 3rd-Party apps:

`pm list packages -3`

- List apps matching specific keywords:

`pm list packages {{keyword1 keyword2 ...}}`

- Display a path of the APK of a specific app:

`pm path {{app}}`
