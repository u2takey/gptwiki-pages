# doskey 
## chatgpt 
The “doskey” command is used in the Microsoft Windows operating system to create macros, edit and recall commands entered previously, and to create new command prompt commands. 

When doskey is executed in a command prompt window, it starts the command line utility that allows you to define and edit macros, and view or modify previous commands entered.

Here are some of the most commonly used options with doskey command:

1. /REINSTALL - resets all doskey macros and restores default command prompt history
2. /MACROS - displays the list of all currently defined doskey macros
3. /HISTORY - displays the command prompt history
4. /LISTSIZE - sets the number of commands that are displayed in the history list
5. /INSERT - specifies the behavior of the command prompt when text is added to a line in the middle of an existing input
6. /APPEND - specifies the behavior of the command prompt when text is added at the end of the current input line
7. /EXENAME - changes the name of the doskey macro


Overall, the doskey command is a useful tool for users who regularly work with the command prompt in Windows and want to streamline their workflow. 

## tldr 
 
> Manage macros, windows commands and command-lines.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/doskey>.

- List available macros:

`doskey /macros`

- Create a new macro:

`doskey {{name}} = "{{command}}"`

- Create a new macro for a specific executable:

`doskey /exename={{executable}} {{name}} = "{{command}}"`

- Remove a macro:

`doskey {{name}} =`

- Display all commands that are stored in memory:

`doskey /history`

- Save macros to a file for portability:

`doskey /macros > {{path\to\macinit_file}}`

- Load macros from a file:

`doskey /macrofile = {{path\to\macinit_file}}`
