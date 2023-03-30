# whereis 
## chatgpt 
The `whereis` command is a tool that can be used in UNIX-based operating systems to locate the binary, source, and manual pages for a specific command. When executed followed by the name of a command, `whereis` searches for the command in standard directories (/bin, /sbin, /usr/sbin, /usr/bin/, etc.) and optionally displays its paths. 

The output of `whereis` will typically display three types of paths:

1. Binary: This path refers to the executable file responsible for running the command.
2. Source: This path points to the source code of the command, which is typically needed to modify, compile, or troubleshoot the command.
3. Manual: This path indicates where the documentation of a command such as a man page is located.

For example, executing the command `whereis ls` might output the following:
```
ls: /bin/ls /usr/share/man/man1/ls.1.gz
```
This indicates that the `ls` command is located in `/bin/ls` and that its manual page is located in `/usr/share/man/man1/ls.1.gz`. In this example, no source code is available for the `ls` command. 

Overall, the `whereis` command can be useful for users and system administrators alike to locate important system commands and their related files in order to modify, troubleshoot, or better understand how they work. 

## tldr 
 
> Locate the binary, source, and manual page files for a command.
> More information: <https://manned.org/whereis>.

- Locate binary, source and man pages for ssh:

`whereis {{ssh}}`

- Locate binary and man pages for ls:

`whereis -bm {{ls}}`

- Locate source of gcc and man pages for Git:

`whereis -s {{gcc}} -m {{git}}`

- Locate binaries for gcc in `/usr/bin/` only:

`whereis -b -B {{/usr/bin/}} -f {{gcc}}`

- Locate unusual binaries (those that have more or less than one binary on the system):

`whereis -u *`

- Locate binaries that have unusual manual entries (binaries that have more or less than one manual installed):

`whereis -u -m *`
