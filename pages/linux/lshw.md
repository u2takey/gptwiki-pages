# lshw 
## chatgpt 
The command "lshw" is used in the Linux operating system to list and display detailed information about the hardware of the system. This command stands for "list hardware" and is widely used by system administrators, hardware and software engineers, and developers to gather information about the system components.

When you run the "lshw" command, it retrieves information about various hardware elements such as the motherboard, processor, memory, storage devices, USB controllers, network interfaces, video cards, etc. and displays them in a readable format. This allows users to check if a device is properly installed or not and to diagnose any hardware-related issues.

The output of the "lshw" command is divided into sections based on the type of hardware component. The output includes various details about the hardware, such as its manufacturer, model, capacity, speed, serial number, and other related information.

In addition to this basic functionality, the "lshw" command also has several options that users can use to customize its output. For example, the "-short" option can be used to display only a brief summary of the hardware information, while the "-html" option can be used to generate an HTML-formatted report.

Overall, the "lshw" command is a useful tool for anyone working on the Linux platform who needs to gather information about the hardware of their system. 

## tldr 
 
> List detailed information about hardware configurations as root user.
> More information: <https://manned.org/lshw>.

- Launch the GUI:

`sudo lshw -X`

- List all hardware in tabular format:

`sudo lshw -short`

- List all disks and storage controllers in tabular format:

`sudo lshw -class disk -class storage -short`

- Save all network interfaces to an HTML file:

`sudo lshw -class network -html > {{interfaces.html}}`
