# modinfo 
## chatgpt 
The `modinfo` command is a Linux utility that provides information about kernel modules. The command works by reading metadata from the `.ko` or kernel object files, which are loaded into the kernel at runtime. Here is a detailed explanation of its various options and arguments:

Syntax: `modinfo [options] <module name>`

Options:

- `-a` or `--all`: Displays all available information about the module.
- `-F <format string>` or `--format=<format string>`: Displays information in the specified format string.
- `-0` or `--null`: Sets the output delimiter to a null byte instead of a newline character.
- `-k <kernel directory>` or `--kernel-dir=<kernel directory>`: Specifies a custom location for the kernel modules directory. By default, modinfo reads from the currently running kernel's modules directory.
- `-p <parameters>` or `--parameters=<parameters>`: Displays the values of the specified module parameters.

Module name: Specifies the name of the module that you want to get information about. This is typically the file name of the module minus the `.ko` extension.

Here are some examples of the `modinfo` command usage:

To display all available information for the `nvidia` module, run:

```bash
modinfo -a nvidia
```

To get the filename and author of the `nvidia` module, run:

```bash
modinfo -F "filename: %f\nauthor: %a\n" nvidia
```

To get the value of the `modeset` parameter for the `i915` module, run:

```bash
modinfo -p i915 | grep modeset
```

Note that these are just a few examples of the many possible use cases for `modinfo`. The full list of options and arguments can be seen by running `modinfo --help`. 

## tldr 
 
> Extract information about a Linux kernel module.
> More information: <https://manned.org/modinfo>.

- List all attributes of a kernel module:

`modinfo {{kernel_module}}`

- List the specified attribute only:

`modinfo -F {{author|description|license|parm|filename}} {{kernel_module}}`
