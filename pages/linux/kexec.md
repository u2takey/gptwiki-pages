# kexec 
## chatgpt 
kexec is a command-line utility in Unix-like operating systems that allows a user to quickly reboot their system with a new kernel. 

When executed, kexec preloads the new kernel into the system memory, which avoids the time-consuming process of shutting down the system, loading the new kernel, and restarting. Instead, kexec initiates a “soft reboot” by immediately switching to the new kernel and shutting down all old processes.

The syntax for using the kexec command is as follows:

```kexec [-f] [-l] [-p] [-u] [--initrd=initrd] [--command-line=cmdline] [-d] [-H] [-k] [-s] [--no-jump] [--force] [--use-cmdline] kernel-image```

Here are the arguments used in the kexec command:

- **-f, --force:** Forces a kernel reboot even if it is not safe to do so.
- **-l, --load:** Loads kernel and its initrd without rebooting the system.
- **-p, --load-panic:** Loads kernel without reboot, and sets the panic kernel.
- **-u, --unload:** Unloads the previously loaded kernel.
- **--initrd=initrd:** Specifies the initrd to use with the new kernel.
- **--command-line=cmdline:** Specifies the command line options to boot the new kernel with.
- **-d, --no-dt:** Disables the device tree.
- **-H, --use-heap:** Uses the heap for the new kernel image.
- **-k, --kexec-file=file:** Specifies the file to load with kexec.
- **-s, --suspend:** Suspends the system instead of rebooting.
- **--no-jump:** Does not jump into the new kernel.
- **--use-cmdline:** Uses the command line options for the new kernel.

Overall, the kexec command is a useful tool for quickly rebooting a Unix-like system with a new kernel without the need for shutting down the system. 

## tldr 
 
> Directly reboot into a new kernel.
> More information: <https://manned.org/kexec>.

- Load a new kernel:

`kexec -l {{path/to/kernel}} --initrd={{path/to/initrd}} --command-line={{arguments}}`

- Load a new kernel with current boot parameters:

`kexec -l {{path/to/kernel}} --initrd={{path/to/initrd}} --reuse-cmdline`

- Execute a currently loaded kernel:

`kexec -e`

- Unload current kexec target kernel:

`kexec -u`
