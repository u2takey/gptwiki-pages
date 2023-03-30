# batch 
## chatgpt 
The command "batch" is a Windows command used to execute commands or scripts at a specified time or when system resources are available. When the "batch" command is executed, it creates a new command window and enters a batch scripting mode that allows the user to enter one or more commands to execute in sequence or as a single block.

To use the "batch" command, first, open the Command Prompt by pressing the Windows key + R, typing "cmd" and pressing Enter. Then, type "batch" followed by any additional options or commands. Some of the most common options include:

- /c - executes the command and then terminates
- /k - executes the command and leaves the command window open
- /d - changes the default drive to the specified drive

Once the options are specified, the user can enter any number of commands that they want to execute. These commands can be batch scripts or individual commands separated by the "&" command.

For example, to create a batch file that opens a web browser at a specified time, the following commands would be used:

1. Open Notepad or any text editor
2. Type "@echo off" to disable displaying the commands on the screen
3. Type "start iexplore.exe" to open Internet Explorer
4. Save the file with a .bat extension, e.g. OpenBrowser.bat
5. Open the Command Prompt and navigate to the location where the file is saved
6. Type "batch OpenBrowser.bat" to execute the batch file and open the web browser.

The "batch" command is a powerful tool for automating system tasks and executing commands at a specific time or event. Its flexibility makes it a valuable tool for system administrators and power users alike. 

## tldr 
 
> Execute commands at a later time when the system load levels permit.
> Service atd (or atrun) should be running for the actual executions.
> More information: <https://manned.org/batch>.

- Execute commands from standard input (press `Ctrl + D` when done):

`batch`

- Execute a command from standard input:

`echo "{{./make_db_backup.sh}}" | batch`

- Execute commands from a given file:

`batch -f {{path/to/file}}`
