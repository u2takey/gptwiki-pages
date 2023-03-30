# coredumpctl 
## chatgpt 
The `coredumpctl` command is a utility that allows users to manage and interact with system core dumps (also known as core files or crash dumps). Core dumps are files that contain a snapshot of the memory and registers of a running program at the time it crashed. They can be used by developers to diagnose and fix software bugs, as well as by system administrators to identify and troubleshoot system crashes.

Here's a more detailed look at the various options and subcommands available with `coredumpctl`:

- `coredumpctl list`: displays a list of available core dumps, including their timestamp and PID (process identifier).
- `coredumpctl info <PID>`: displays detailed information about a specific core dump with the given PID, such as the program name, executable path, and signal that triggered the crash.
- `coredumpctl info <filename>`: displays detailed information about a specific core dump with the given filename or path.
- `coredumpctl dump <PID>`: saves the contents of a specific core dump to a file in the current directory. The resulting file can then be analyzed using a debugger or other diagnostic tool.
- `coredumpctl gdb <PID>`: launches the GNU Debugger (GDB) and loads the specified core dump for analysis. This option requires that GDB is installed on the system.
- `coredumpctl debug <PID>`: launches a new instance of the crashed program using the specified core dump as input. This can be useful for replicating the crash and testing potential fixes.
- `coredumpctl disable`: disables the collection of core dumps on the system.
- `coredumpctl enable`: re-enables the collection of core dumps on the system.
- `coredumpctl status`: displays the current status of core dump collection, including whether it is enabled or disabled and the maximum size allowed for a single dump.

Overall, coredumpctl is a powerful tool for managing and analyzing system core dumps, and can be used by developers and system administrators alike to diagnose and resolve issues with software and hardware. 

## tldr 
 
> Retrieve and process saved core dumps and metadata.
> More information: <https://www.freedesktop.org/software/systemd/man/coredumpctl.html>.

- List all captured core dumps:

`coredumpctl list`

- List captured core dumps for a program:

`coredumpctl list {{program}}`

- Show information about the core dumps matching a program with `PID`:

`coredumpctl info {{PID}}`

- Invoke debugger using the last core dump of a program:

`coredumpctl debug {{program}}`

- Extract the last core dump of a program to a file:

`coredumpctl --output={{path/to/file}} dump {{program}}`
