# lslocks 
## chatgpt 
The 'lslocks' command is used to list information about all currently held file locks. It displays a list of files that are locked by processes, along with detailed information about the types of locks that have been placed on them.

Syntax: `lslocks [options]`

Some common options are:

- `-a` : Displays information about all locks, including those held by system processes.
- `-c` : Shows the output in CSV format.
- `-d` : Shows detailed information about the locks, including the PID of the process holding the lock.
- `-u` : Displays locks held by the specified user.

The output of the 'lslocks' command typically includes the name of the locked file, the process ID of the process holding the lock, the type of lock (read or write), and the offset and length of the locked region within the file.

Example usage: 

`lslocks -d /home/user/Documents/file.txt`

This command will display detailed information about all locks on the file.txt file located in /home/user/Documents/. The output will include the PID of the process holding the lock, the type of lock, and the offset and length of the locked region within the file. 

## tldr 
 
> List local system locks.
> More information: <https://manned.org/lslocks>.

- List all local system locks:

`lslocks`

- List locks with defined column headers:

`lslocks --output {{PID}},{{COMMAND}},{{PATH}}`

- List locks producing a raw output (no columns), and without column headers:

`lslocks --raw --noheadings`

- List locks by PID input:

`lslocks --pid {{PID}}`

- List locks with JSON output to `stdout`:

`lslocks --json`
