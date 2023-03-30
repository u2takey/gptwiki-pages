# grub-file 
## chatgpt 
I'm sorry, but the command "grub-file" is not a valid command in Linux or Unix systems. Can you provide more context or details about where you encountered this command or what you are trying to achieve? This would help me to provide a better answer or solution. 

## tldr 
 
> Check if a file is of a specific bootable image type.
> More information: <https://manned.org/grub-file>.

- Check if a file is an ARM EFI image:

`grub-file --is-arm-efi {{path/to/file}}`

- Check if a file is an i386 EFI image:

`grub-file --is-i386-efi {{path/to/file}}`

- Check if a file is an x86_64 EFI image:

`grub-file --is-x86_64-efi {{path/to/file}}`

- Check if a file is an ARM image (Linux kernel):

`grub-file --is-arm-linux {{path/to/file}}`

- Check if a file is an x86 image (Linux kernel):

`grub-file --is-x86-linux {{path/to/file}}`

- Check if a file is an x86_64 XNU image (Mac OS X kernel):

`grub-file --is-x86_64-xnu {{path/to/file}}`