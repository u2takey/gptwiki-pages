# fakeroot 
## chatgpt 
The `fakeroot` command creates a virtual root file system that simulates root privileges without actually granting them. 

When you execute a command with `fakeroot` prefix, it intercepts and manipulates the system's file i/o calls on the fly using a library called `libfakeroot`. This creates a fake root environment where all the file operations outside this environment are transparently redirected to the fakeroot's internal file storage, and the fake root filesystem can be accessed, modified, and deleted without having root privileges.

This is useful in situations where you need to create a package or run a script that requires root privileges but you don't have access to a root account. For example, you can use `fakeroot` to create a Debian package from files that you don't actually have permission to modify.

In summary, `fakeroot` creates a simulated root environment that can be used to execute commands with root privileges without actually granting those privileges, which is useful when you don't have root access. 

## tldr 
 
> Run a command in an environment faking root privileges for file manipulation.
> More information: <https://manpages.debian.org/latest/fakeroot/fakeroot.1.html>.

- Start the default shell as fakeroot:

`fakeroot`

- Run a command as fakeroot:

`fakeroot -- {{command}} {{command_arguments}}`

- Run a command as fakeroot and save the environment to a file on exit:

`fakeroot -s {{path/to/file}} -- {{command}} {{command_arguments}}`

- Load a fakeroot environment and run a command as fakeroot:

`fakeroot -i {{path/to/file}} -- {{command}} {{command_arguments}}`

- Run a command keeping the real ownership of files instead of pretending they are owned by root:

`fakeroot --unknown-is-real -- {{command}} {{command_arguments}}`

- Display help:

`fakeroot --help`
