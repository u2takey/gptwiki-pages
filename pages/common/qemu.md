# qemu 
## chatgpt 
QEMU (Quick EMUlator) is a free and open-source software that allows users to emulate a complete computer system. It can emulate various architectures, including x86, ARM, MIPS, and PowerPC.

Here are some common commands used with QEMU:

1. `qemu-system-x86_64`: This command starts the QEMU virtual machine and specifies the target architecture as x86_64, which is commonly used in modern PCs.

2. `-hda <disk_image>`: This option specifies the hard disk image that will be used by the virtual machine.

3. `-cdrom <cdrom_image>`: This option specifies the CD/DVD-ROM image that will be used by the virtual machine.

4. `-boot <boot_order>`: This option specifies the boot order of the virtual machine, which can be set to CD-ROM first, hard disk second, or floppy disk first.

5. `-m <memory_size>`: This option specifies the amount of memory that will be allocated to the virtual machine.

6. `-curses`: This option starts the virtual machine in a terminal window with a text-based interface.

7. `-k <keymap>`: This option specifies the keyboard layout for the virtual machine.

8. `-enable-kvm`: This option enables KVM (Kernel-based Virtual Machine), which is a Linux kernel module that allows faster virtualization by using hardware virtualization extensions.

Overall, QEMU provides a versatile and powerful tool for emulating various architectures and running different operating systems on them. Its flexible options and multiple features make it a popular choice for developers, hobbyists, and researchers alike. 

## tldr 
 
> Generic machine emulator and virtualizer.
> Supports a large variety of CPU architectures.
> More information: <https://www.qemu.org>.

- Boot from image emulating i386 architecture:

`qemu-system-i386 -hda {{image_name.img}}`

- Boot from image emulating x64 architecture:

`qemu-system-x86_64 -hda {{image_name.img}}`

- Boot QEMU instance with a live ISO image:

`qemu-system-i386 -hda {{image_name.img}} -cdrom {{os_image.iso}} -boot d`

- Specify amount of RAM for instance:

`qemu-system-i386 -m 256 -hda image_name.img -cdrom os-image.iso -boot d`

- Boot from physical device (e.g. from USB to test bootable medium):

`qemu-system-i386 -hda /dev/{{storage_device}}`
