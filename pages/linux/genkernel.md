# genkernel 
## chatgpt 
Genkernel is a command-line tool for generating an initramfs file for Linux kernel boot. It automates the process of configuring and compiling the kernel, as well as building an initial RAM disk image that contains essential drivers and tools needed for booting the system.

Here are some of the key features and options of the genkernel command:

- Configuration: Genkernel reads the system's kernel configuration file (usually located at /usr/src/linux/.config) to determine the settings and options to use for building the kernel. It also allows the user to customize various parameters like kernel version, architecture, target device, compression method, and others.

- Compilation: Genkernel uses the standard kernel build process (make) to compile the kernel source code into a binary executable file. It handles the dependencies, modules, and firmware files automatically, based on the selected configuration options.

- Initramfs creation: After compiling the kernel, Genkernel runs a set of scripts to create the initramfs file, which contains the minimum set of files and utilities required to boot the system. This includes the kernel image itself, the necessary device drivers, the filesystem tools, and the boot loader (GRUB or LILO).

- Customization: Genkernel allows users to customize the initramfs image by adding extra files and directories to it, modifying the boot scripts, or specifying additional kernel parameters. This can be useful for integrating third-party modules, drivers or utilities, or for debugging purposes.

- Usage: Genkernel is typically run as root or with sudo privileges, using the genkernel command followed by various options and arguments. Some common options include "--menuconfig" (to interactively select kernel options), "--no-clean" (to avoid deleting the temporary build files), "--install" (to install the new kernel and initramfs images), "--mrproper" (to clean up the kernel sources), and many others.

Overall, the genkernel command simplifies the otherwise complex and error-prone process of building and deploying a custom Linux kernel, especially for novice or non-technical users. However, it is not suitable for advanced users who require fine-grained control over the kernel configuration and build process. 

## tldr 
 
> Gentoo Linux utility to compile and install kernels.
> More information: <https://wiki.gentoo.org/wiki/Genkernel>.

- Automatically compile and install a generic kernel:

`sudo genkernel all`

- Build and install the bzImage|initramfs|kernel|ramdisk only:

`sudo genkernel {{bzImage|initramfs|kernel|ramdisk}}`

- Apply changes to the kernel configuration before compiling and installing:

`sudo genkernel --menuconfig all`

- Generate a kernel with a custom name:

`sudo genkernel --kernname={{custom_name}} all`

- Use a kernel source outside the default directory `/usr/src/linux`:

`sudo genkernel --kerneldir={{path/to/directory}} all`
