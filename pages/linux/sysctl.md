# sysctl 
## chatgpt 
The `sysctl` command in Linux is used to modify kernel parameters at runtime. It allows users to view and customize kernel parameters that affect the behavior of the operating system. 

The command accepts names of kernel parameters as arguments, modifies the values associated with the specified parameters and retrieves information about the current kernel parameter values. By default, this command sets kernel parameters temporarily, and once the system reboots or restarts, the settings are lost unless they are made persistent through system configuration files.

Here are some common uses of `sysctl` command:

- To view all kernel parameters, use the command `sysctl -a`
- To view a specific kernel parameter, use the command `sysctl <parameter_name>`
- To set a kernel parameter temporarily, use the command `sysctl -w <parameter_name>=<value>`
- To set a kernel parameter persistently, set it in the appropriate configuration file like `/etc/sysctl.conf` or a file in `/etc/sysctl.d/`

It is important to note that modifying kernel parameters can have a significant impact on the system's behavior and stability. Users are advised to exercise caution while using the `sysctl` command, and only perform modifications after carefully reviewing the kernel parameter settings and their effects on the system. 

## tldr 
 
> List and change kernel runtime variables.
> More information: <https://manned.org/sysctl.8>.

- Show all available variables and their values:

`sysctl -a`

- Set a changeable kernel state variable:

`sysctl -w {{section.tunable}}={{value}}`

- Get currently open file handlers:

`sysctl fs.file-nr`

- Get limit for simultaneous open files:

`sysctl fs.file-max`

- Apply changes from `/etc/sysctl.conf`:

`sysctl -p`
