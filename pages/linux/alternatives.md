# alternatives 
## chatgpt 
The "alternatives" command in Linux is used to manage symbolic links that are used to select default commands for a particular user or system. 

It is primarily used to provide multiple versions of a program on a single system, allowing users to switch between different versions of a program without having to change the program name or location.

The syntax of the alternatives command is as follows:

```
alternatives [options] <command>
```

"options" refer to any arguments or options that can be passed along with the command.

"command" refers to the specific command that you want to manage using alternatives.

Some useful options available with the alternatives command are:

- "--config" - This option displays a menu of available alternatives for the specified command and allows the user to choose which one to use as the default.

- "--display" - This option displays the currently selected alternative for the specified command.

- "--install" - This option adds a new alternative to the system.

- "--remove" - This option removes an alternative from the system.

Overall, the alternatives command is designed to make it easier to manage multiple versions of programs on a Linux system, allowing for greater flexibility and control over which version of a particular command is used. 

## tldr 
 
> This command is an alias of `update-alternatives`.
> More information: <https://manned.org/alternatives>.

- View documentation for the original command:

`tldr update-alternatives`
