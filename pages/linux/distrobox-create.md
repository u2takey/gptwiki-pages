# distrobox-create 
## chatgpt 
Unfortunately, as an AI language model, I am not aware of any specific command named "distrobox-create". It could be a custom command created by an individual or organization. 

However, in general, "distro" refers to a distribution, usually a Linux distribution, which is a version or variant of the Linux operating system. "Box" often refers to a virtual machine or container.

So, "distrobox-create" may be a command that creates a virtual machine or container for a particular Linux distribution. Without further context, it is difficult to provide a more detailed explanation. 

## tldr 
 
> Create a distrobox container. See also: `tldr distrobox`.
> The container created will be tightly integrated with the host, allowing sharing of the user's HOME directory, external storage, external USB devices, graphical apps (X11/Wayland), and audio.
> More information: <https://distrobox.privatedns.org/usage/distrobox-create.html>.

- Create a distrobox container using the Ubuntu image:

`distrobox-create {{container_name}} --image {{ubuntu:latest}}`

- Clone a distrobox container:

`distrobox-create --clone {{container_name}} {{cloned_container_name}}`
