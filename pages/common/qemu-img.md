# qemu-img 
## chatgpt 
QEMU-img is a command-line tool that is used for creating, converting, and editing disk image files in a variety of formats. It is related to the QEMU virtualization software, which allows users to run multiple virtual machines on a single physical machine.

Some of the most commonly used QEMU-img commands include:

1. creating a new disk image - this can be done with the "create" command followed by the desired disk image format and file name.

Example: qemu-img create -f qcow2 mydisk.qcow2 10G

This creates a new QCOW2 format disk image called "mydisk.qcow2" with a size of 10GB.

2. converting between different disk image formats - QEMU-img can convert disk images between different formats, such as raw, VDI, VMDK, and others.

Example: qemu-img convert -f raw -O qcow2 mydisk.img mydisk.qcow2

This command converts a raw format disk image called "mydisk.img" into a QCOW2 format disk image called "mydisk.qcow2".

3. resizing an existing disk image - QEMU-img can also be used to resize an existing disk image to a new size.

Example: qemu-img resize mydisk.qcow2 +5G

This command increases the size of the "mydisk.qcow2" disk image by 5GB.

Overall, QEMU-img is a powerful and flexible tool that can be used for a variety of tasks related to disk image files in virtualization environments. 

## tldr 
 
> Tool for Quick Emulator Virtual HDD image creation and manipulation.
> More information: <https://qemu.readthedocs.io/en/latest/tools/qemu-img.html>.

- Create disk image with a specific size (in gigabytes):

`qemu-img create {{image_name.img}} {{gigabytes}}G`

- Show information about a disk image:

`qemu-img info {{image_name.img}}`

- Increase or decrease image size:

`qemu-img resize {{image_name.img}} {{gigabytes}}G`

- Dump the allocation state of every sector of the specified disk image:

`qemu-img map {{image_name.img}}`

- Convert a VMware .vmdk disk image to a KVM .qcow2 disk image:

`qemu-img convert -f {{vmdk}} -O {{qcow2}} {{path/to/file/foo.vmdk}} {{path/to/file/foo.qcow2}}`
