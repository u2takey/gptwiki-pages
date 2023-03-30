# flock 
## chatgpt 
The `flock` command is a Linux utility that allows a user to lock a specified file or directory to prevent other programs or users from accessing it. The basic syntax of the `flock` command is as follows:

```
flock [OPTIONS] <FILE/DIR> <COMMAND>
```

- `[OPTIONS]`: This argument specifies any additional options or flags that modify the behavior of the `flock` command. Some common options include `-c`, which runs the specified command with the lock held in background and `-n`, which attempts to obtain a non-blocking lock on the file or directory.

- `<FILE/DIR>`: This argument specifies the file or directory to be locked by the `flock` command.

- `<COMMAND>`: This argument specifies the command to be executed after the file or directory has been locked. The command can be any valid Linux command or script.

When the `flock` command is run with a file or directory argument, it creates a file-based lock on that file or directory. This lock prevents any other processes or users from accessing or modifying the file or directory until the lock is released. This can be especially useful for preventing multiple instances of a program from accessing the same file or directory simultaneously.

For example, to lock the file `/var/log/messages` and run the `tail` command to display the last 10 lines of the file, the following command can be used:

```
flock /var/log/messages -c "tail -n 10 /var/log/messages"
```

This will run the `tail` command with a lock held on the `/var/log/messages` file, ensuring that no other programs can modify the file while the `tail` command is running. Once the `tail` command completes, the lock is automatically released.

In summary, the `flock` command is a useful utility for managing file-based locks in Linux, allowing users to prevent other processes from accessing or modifying critical files or directories during their own operations. 

## tldr 
 
> Manage locks from shell scripts.
> It can be used to ensure that only one process of a command is running.
> More information: <https://manned.org/flock>.

- Run a command with a file lock as soon as the lock is not required by others:

`flock {{path/to/lock.lock}} --command "{{command}}"`

- Run a command with a file lock, and exit if the lock doesn't exist:

`flock {{path/to/lock.lock}} --nonblock --command "{{command}}"`

- Run a command with a file lock, and exit with a specific error code if the lock doesn't exist:

`flock {{path/to/lock.lock}} --nonblock --conflict-exit-code {{error_code}} -c "{{command}}"`
