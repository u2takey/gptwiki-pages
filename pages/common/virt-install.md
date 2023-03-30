# virt-install 
## chatgpt 
virt-install is a command-line tool used for creating virtual machines (VMs) on a KVM hypervisor. This command is used to install and configure a new guest machine using the command-line interface. Below are the detailed explanations of the different parameters of the virt-install command:

- --name: The name of the virtual machine you want to create.
- --ram: The amount of RAM to assign to the virtual machine in megabytes.
- --vcpus: The number of virtual CPUs to assign to the virtual machine.
- --disk: Options for setting up the primary disk of the VM, including path, size, and format.
- --cdrom: The path to the ISO file for the operating system to be installed.

There are other optional parameters that can be used with virt-install, such as network configuration, password settings, and more.

An example of the virt-install command is:

```
virt-install --name=my_vm --ram=2048 --vcpus=2 --disk path=/var/lib/virt/images/my_vm.qcow2,size=20 --cdrom=my_os.iso
```

This will create a new virtual machine named "my_vm" with 2 GB of RAM, 2 virtual CPUs, a 20 GB virtual disk with the qcow2 format, and will install the operating system from the "my_os.iso" file. 

## tldr 
 
> Create virtual machines with libvirt and begin OS installation.
> More information: <https://virt-manager.org/>.

- Create a virtual machine with 1 GB RAM and 12 GB storage and start a Debian installation:

`virt-install --name {{vm_name}} --memory {{1024}} --disk path={{path/to/image.qcow2}},size={{12}} --cdrom {{path/to/debian.iso}}`

- Create a x86-64, KVM-accelerated, UEFI-based virtual machine with the Q35 chipset, 4 GiB RAM, 16 GiB RAW storage, and start a Fedora installation:

`virt-install --name {{vm_name}} --arch {{x86_64}} --virt-type {{kvm}} --machine {{q35}} --boot {{uefi}} --memory {{4096}} --disk path={{path/to/image.raw}},size={{16}} --cdrom {{path/to/fedora.iso}}`

- Create a diskless live virtual machine without an emulated sound device or a USB controller. Don't start an installation and don't autoconnect to console but attach a cdrom to it (might be useful for when using a live CD like tails):

`virt-install --name {{vm_name}} --memory {{512}} --disk {{none}} --controller {{type=usb,model=none}} --sound {{none}} --autoconsole {{none}} --install {{no_install=yes}}  --cdrom {{path/to/tails.iso}}`

- Create a virtual machine with 16 GiB RAM, 250 GiB storage, 8 cores with hyperthreading, a specific CPU topology, and a CPU model that shares most features with the host CPU:

`virt-install --name {{vm_name}} --cpu {{host-model}},topology.sockets={{1}},topology.cores={{4}},topology.threads={{2}} --memory {{16384}} --disk path={{path/to/image.qcow2}},size={{250}} --cdrom {{path/to/debian.iso}}`

- Create a virtual machine and kickstart an automated deployment based on Fedora 35 using only remote resources (no ISO required):

`virt-install --name {{vm_name}} --memory {{2048}} --disk path={{path/to/image.qcow2}},size={{20}} --location={{https://download.fedoraproject.org/pub/fedora/linux/releases/35/Everything/x86_64/os/}} --extra-args={{"inst.ks=https://path/to/valid/kickstart.org"}}`
