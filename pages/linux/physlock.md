# physlock 
## chatgpt 
The physlock command is a Linux terminal command that allows the locking of all physical terminals on a machine. 

When executed, the physlock command will lock all terminals that have physical access to the machine. This means that if anyone tries to access the machine physically through a keyboard or mouse, they will not be able to bypass the lock and gain access without entering a password. 

This command can be particularly useful in situations where there are multiple users who share the same machine, or in situations where the machine is located in a public space and needs to be secured. The physlock command allows the user to ensure that only authorized individuals are able to access the machine directly. 

To execute the physlock command, type "physlock" into the terminal and press enter. This will lock all physical terminals on the machine. To unlock the terminals, the user must enter the password that was set when the lock was initiated. 

## tldr 
 
> Lock all consoles and virtual terminals.
> More information: <http://github.com/muennich/physlock>.

- Lock every console (require current user or root to unlock):

`physlock`

- Mute kernel messages on console while locked:

`physlock -m`

- Disable SysRq mechanism while locked:

`physlock -s`

- Display a message before the password prompt:

`physlock -p "{{Locked!}}"`

- Fork and detach physlock (useful for suspend or hibernate scripts):

`physlock -d`
