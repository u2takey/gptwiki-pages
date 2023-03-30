# ctrlaltdel 
## chatgpt 
The command "Ctrl+Alt+Delete" is a keyboard shortcut used on computers running the Windows operating system. It is used to open the "Windows Security" dialog box which provides options for users to lock the computer, switch user accounts, change a password, open Task Manager or shut down or restart the computer.

The "Ctrl" key is located in the bottom left or right corner of most keyboards and is short for "control". When held down and pressed in combination with the other keys, it activates a specific command.

The "Alt" key is also located in the bottom left or right corner of most keyboards and is short for "alternative". When held down and pressed in combination with other keys, it provides an alternative function.

The "Delete" key is located in the top right corner of most keyboards and is used to delete characters or undo actions in many programs.

To use this keyboard shortcut, press and hold down "Ctrl" and "Alt" at the same time and then press "Delete" once. This will bring up the "Windows Security" dialog box, where you can perform the desired action. 

## tldr 
 
> Utility to control what happens when CTRL+ALT+DEL is pressed.
> More information: <https://manned.org/ctrlaltdel>.

- Get current setting:

`ctrlaltdel`

- Set CTRL+ALT+DEL to reboot immediately, without any preparation:

`sudo ctrlaltdel hard`

- Set CTRL+ALT+DEL to reboot "normally", giving processes a chance to exit first (send SIGINT to PID1):

`sudo ctrlaltdel soft`
