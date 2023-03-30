# xmount 
## chatgpt 
xmount is a command-line tool used to mount disk images and virtual machine images in read-only or read-write mode. It supports a variety of image formats, including DMG, VMDK, VDI, ISO, and more.

The basic syntax for xmount is:

xmount [options] <image-file> <mount-point>

The image-file parameter specifies the disk image or virtual machine image that you want to mount, while the mount-point parameter specifies the directory in which the image should be mounted.

Options can be used to specify the mount mode, file system type, compression type, encryption, etc.

For example:

xmount -in ewf image.E01 /mnt/image

This command mounts a disk image file named image.E01 in EWF format in read-only mode at the mount point /mnt/image.

Another example:

xmount -t raw -o loop,offset=512 image.dd /mnt/image

This command mounts a disk image file named image.dd in raw format as read-only with the loop option and an offset value of 512 at the mount point /mnt/image.

Overall, xmount is a powerful tool for working with disk images and virtual machine images, providing a range of useful features and options. 

## tldr 
 
> Convert on-the-fly between multiple input and output hard disk image types with optional write cache support.
> Creates a virtual file system using FUSE (Filesystem in Userspace) that contains a virtual representation of the input image.
> More information: <https://manned.org/xmount>.

- Mount a `.raw` image file into a DMG container file:

`xmount --in {{raw}} {{path/to/image.dd}} --out {{dmg}} {{mountpoint}}`

- Mount an EWF image file with write-cache support into a VHD file to boot from:

`xmount --cache {{path/to/cache.ovl}} --in {{ewf}} {{path/to/image.E??}} --out {{vhd}} {{mountpoint}}`

- Mount the first partition at sector 2048 into a new `.raw` image file:

`xmount --offset {{2048}} --in {{raw}} {{path/to/image.dd}} --out {{raw}} {{mountpoint}}`
