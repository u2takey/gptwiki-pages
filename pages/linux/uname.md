# uname 
## chatgpt 
The `uname` command is a command-line utility in Unix and Unix-like operating systems that is used to display certain system information, specifically regarding the system's kernel and operating system architecture. 

When the `uname` command is executed without any options or arguments, it will display the name of the operating system:

```
$ uname
Linux
```

However, there are several options (also known as flags or switches) that can be used with the `uname` command to display additional details about the system. Some of the most commonly used options are:

- `-a` (or `--all`): Displays all available system information, including the kernel name and version, the machine architecture, the operating system name and version, and more:

```
$ uname -a
Linux mycomputer 5.8.0-55-generic #62~20.04.1-Ubuntu SMP Fri Jun 25 07:58:11 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux
```

- `-s` (or `--kernel-name`): Displays the name of the operating system's kernel:

```
$ uname -s
Linux
```

- `-r` (or `--kernel-release`): Displays the release number of the operating system's kernel:

```
$ uname -r
5.8.0-55-generic
```

- `-m` (or `--machine`): Displays the system's machine or hardware architecture:

```
$ uname -m
x86_64
```

- `-o` (or `--operating-system`): Displays the name of the operating system:

```
$ uname -o
GNU/Linux
```

Overall, the `uname` command is a simple but useful utility for retrieving system information, and can be used in shell scripts and other automated processes to determine system properties that can be used to make decisions throughout the script. 

## tldr 
 
> Uname prints information about the machine and operating system it is run on.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/uname-invocation.html>.

- Print all information:

`uname --all`

- Print the current kernel name:

`uname --kernel-name`

- Print the current network node host name:

`uname --nodename`

- Print the current kernel release:

`uname --kernel-release`

- Print the current kernel version:

`uname --kernel-version`

- Print the current machine hardware name:

`uname --machine`

- Print the current processor type:

`uname --processor`

- Print the current operating system name:

`uname --operating-system`
