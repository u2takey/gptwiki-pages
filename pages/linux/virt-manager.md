# virt-manager 
## chatgpt 
The virt-manager command launches a graphical user interface (GUI) for managing virtual machines on a host system. virt-manager is a tool that provides a convenient way to create and configure virtual machines using QEMU, KVM, or Xen virtualization technologies.

When you run the virt-manager command, it launches the virt-manager application, which allows you to perform a variety of virtual machine management tasks, including creating new virtual machines, starting and stopping virtual machines, and managing virtual storage devices.

The virt-manager GUI has several panes that provide access to different virtualization management functions. The main window provides an overview of all the virtual machines that are running on the host system. You can launch and access the management interface for each virtual machine by selecting it from the list.

The left-hand pane shows the available virtual machines and their configuration. You can create new virtual machines, edit and configure existing ones, and delete virtual machines from this pane. The right-hand pane provides details about the selected virtual machine, such as hardware information, network configurations, and storage devices.

Overall, the virt-manager command provides a convenient and user-friendly way to manage virtual machines on a host system using a graphical interface. 

## tldr 
 
> CLI launcher for virt-manager, a desktop user interface for managing KVM and Xen virtual machines and LXC containers.
> More information: <https://manpages.ubuntu.com/manpages/man1/virt-manager.1.html>.

- Launch virt-manager:

`virt-manager`

- Connect to a hypervisor:

`virt-manager --connect {{hypervisor_uri}}`

- Don't fork virt-manager process into background on startup:

`virt-manager --no-fork`

- Print debug output:

`virt-manager --debug`

- Open the "New VM" wizard:

`virt-manager --show-domain-creator`

- Show domain details window:

`virt-manager --show-domain-editor {{name|id|uuid}}`

- Show domain performance window:

`virt-manager --show-domain-performance {{name|id|uuid}}`

- Show connection details window:

`virt-manager --show-host-summary`
