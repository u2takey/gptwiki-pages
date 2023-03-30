# am 
## chatgpt 
The "am" command is the abbreviation of "Activity Manager" and is a command-line tool available on Android devices, used to manage and control Android package manager (pm) commands. By using "am," you can start and stop any activity, broadcast an intent, display a list of recent activities, or send an intent from one application to another. The basic syntax of the "am" command is as follows:

am [subcommand] [options] [component]

Here, the subcommand can be any one of the following: 

1. start: to start an activity
2. broadcast: to broadcast an intent to the system
3. instrument: to start an Instrumentation class to run tests
4. startservice: to start a service
5. dumpheap: to dump the memory heap of a running process to a file
6. profile: to start and stop method profiling

The option parameter is used to specify additional options to the subcommand, and the component parameter is used to specify the component to perform the subcommand on.

For example, the following command is used to start an activity:

am start -n com.example/com.example.MainActivity

Here, "com.example" is the package name and "com.example.MainActivity" is the fully-qualified name of the activity you want to start. This will open the specified activity on the device. 

In summary, the "am" command in Android is a powerful tool that allows developers to perform a variety of tasks related to activity and package management on Android devices through the command line. 

## tldr 
 
> Android activity manager.
> More information: <https://developer.android.com/studio/command-line/adb#am>.

- Start a specific activity:

`am start -n {{com.android.settings/.Settings}}`

- Start an activity and pass [d]ata to it:

`am start -a {{android.intent.action.VIEW}} -d {{tel:123}}`

- Start an activity matching a specific action and [c]ategory:

`am start -a {{android.intent.action.MAIN}} -c {{android.intent.category.HOME}}`

- Convert an intent to a URI:

`am to-uri -a {{android.intent.action.VIEW}} -d {{tel:123}}`
