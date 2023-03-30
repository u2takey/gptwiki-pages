# bundletool 
## chatgpt 
The `bundletool` command is a tool used to build, test, and manipulate Android App Bundles. It is part of the Android SDK and can be installed on your computer by downloading and installing the latest version of the Android Studio.

Here are the main features of the `bundletool` command:

- Build: it can be used to build an Android App Bundle from an existing APK, app module or set of dynamic feature modules. It also allows you to customize your app bundle by specifying the modules and their configuration that you want to include. You can use the `build-bundle` subcommand for this purpose.

- Test: it can be used to test your app bundle on different devices or configurations. You can use the `test` subcommand to install and run your bundle on a connected device or an emulator.

- Deploy: it can be used to deploy your app bundle to the Google Play Store, a private app catalog or to devices directly. You can use the `deploy` subcommand to upload your bundle to the Google Play Store, generate APKs for sideloading or generate a set of APKs for every device configuration in your bundle.

- Inspect: it can be used to inspect the contents of your app bundle and get information about its modules, configuration, and size. You can use the `dump` subcommand to get information about your bundle or the `extract-apks` subcommand to extract the APKs from your bundle.

Overall, the `bundletool` command is a very powerful tool that allows you to manage the lifecycle of your app bundle and make sure that it is optimized for distribution and performance. 

## tldr 
 
> Command-line tool to manipulate Android Application Bundles.
> Some subcommands such as `bundletool validate` have their own usage documentation.
> More information: <https://developer.android.com/studio/command-line/bundletool>.

- Display help for a subcommand:

`bundletool help {{subcommand}}`

- Generate APKs from an application bundle (prompts for keystore password):

`bundletool build-apks --bundle={{path/to/bundle.aab}} --ks={{path/to/key.keystore}} --ks-key-alias={{key_alias}} --output={{path/to/file.apks}}`

- Generate APKs from an application bundle giving the keystore password:

`bundletool build-apks --bundle={{path/to/bundle.aab}} --ks={{path/to/key.keystore}} --ks-key-alias={{key_alias}} –ks-pass={{pass:the_password}} --output={{path/to/file.apks}}`

- Generate APKs including only one single APK for universal usage:

`bundletool build-apks --bundle={{path/to/bundle.aab}} --mode={{universal}} --ks={{path/to/key.keystore}} --ks-key-alias={{key_alias}} --output={{path/to/file.apks}}`

- Install the right combination of APKs to an emulator or device:

`bundletool install-apks --apks={{path/to/file.apks}}`

- Estimate the download size of an application:

`bundletool get-size total --apks={{path/to/file.apks}}`

- Generate a device specification JSON file for an emulator or device:

`bundletool get-device-spec --output={{path/to/file.json}}`

- Verify a bundle and display detailed information about it:

`bundletool validate --bundle={{path/to/bundle.aab}}`
