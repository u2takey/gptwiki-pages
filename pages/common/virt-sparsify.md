# virt-sparsify 
## chatgpt 
`virt-sparsify` is a command-line tool used to shrink the size of virtual machine images in the QEMU/KVM format. It creates a new image with only the used blocks of the original image, freeing up unused space. The command works by using the `sparse` format for the new image, making it use less space on the host machine.

The `virt-sparsify` command has several options to specify the input and output files, the format of the output file, and the compression level. Some useful options are:

- `-o, --output`: Specifies the path of the output file.
- `-q, --quiet`: Suppresses progress messages.
- `-c, --compress`: Enables compression of the output file.

It is important to note that `virt-sparsify` does not modify the original image, and the new image should be used instead to benefit from the space savings. It is also recommended to run `virt-sparsify` on powered off virtual machines to avoid data corruption.

Overall, the `virt-sparsify` command is a powerful tool to shrink virtual machine images and reduce storage usage. 

## tldr 
 
> Make virtual machine drive images thin-provisioned.
> NOTE: Use only for offline machines to avoid data corruption.
> More information: <https://libguestfs.org>.

- Create a sparsified compressed image without snapshots from an unsparsified one:

`virt-sparsify --compress {{path/to/image.qcow2}} {{path/to/image_new.qcow2}}`

- Sparsify an image in-place:

`virt-sparsify --in-place {{path/to/image.img}}`
