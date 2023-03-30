# sdkmanager 
## chatgpt 
The `sdkmanager` command is a tool that is used in Android development to manage the Android Software Development Kit (SDK). It lets developers download and manage the required SDK components, tools, and platforms for developing Android apps.

The `sdkmanager` command is a command-line tool and is typically used from the terminal or command prompt. It is available as part of the Android SDK command-line tools package.

Here are some examples of how `sdkmanager` can be used:

- To list available SDK packages:

  ```
  sdkmanager --list
  ```

- To install a specific SDK package:

  ```
  sdkmanager "platform-tools" "build-tools;29.0.3" "platforms;android-29"
  ```

  This command installs the platform tools, build tools for version 29.0.3, and the Android SDK platform for version 29.

- To update an existing SDK package:

  ```
  sdkmanager --update "build-tools;29.0.3"
  ```

- To remove an SDK package:

  ```
  sdkmanager --uninstall "platforms;android-29"
  ```

In summary, `sdkmanager` is a command-line tool that lets developers manage the Android SDK and the required components for developing Android apps. It provides commands for installing, updating, and removing SDK packages. 

## tldr 
 
> Tool to install packages for the Android SDK.
> More information: <https://developer.android.com/studio/command-line/sdkmanager>.

- List available packages:

`sdkmanager --list`

- Install a package:

`sdkmanager {{package}}`

- Update every installed package:

`sdkmanager --update`

- Uninstall a package:

`sdkmanager --uninstall {{package}}`
