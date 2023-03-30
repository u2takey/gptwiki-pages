# settings 
## chatgpt 
As an AI language model, I may not be able to determine the context of your question but generally speaking, "settings" in the context of computing refers to the application or system configurations that govern the behavior of a particular application or system. The "settings" command may be used in different contexts depending on the operating system, application, or programming language. In some cases, the "settings" command may be used to view or modify the settings of a particular application or system, while in other cases, it may be used to access or modify the settings of a particular component, module, or library. For instance, in Windows operating systems, the "settings" command may be used to access the settings of the "Control Panel," "Windows Security," "Windows Defender," "Windows Update," "Display," "Network," "System," and many other components. In addition, most modern web browsers have their own settings page that allows users to customize the browser to their preferences, and the browser's settings command may be used to access and modify those settings. Overall, the "settings" command may vary widely based on the context in which it is used. 

## tldr 
 
> Get information about the Android OS.
> More information: <https://adbinstaller.com/commands/adb-shell-settings-5b670d5ee7958178a2955536>.

- Display a list of settings in the `global` namespace:

`settings list {{global}}`

- Get a value of a specific setting:

`settings get {{global}} {{airplane_mode_on}}`

- Set a specific value of a setting:

`settings put {{system}} {{screen_brightness}} {{42}}`

- Delete a specific setting:

`settings delete {{secure}} {{screensaver_enabled}}`
