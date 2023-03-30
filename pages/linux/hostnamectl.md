# hostnamectl 
## chatgpt 
The "hostnamectl" command is used in Linux-based systems to view or set the hostname of the system. 

When executing this command without any arguments, it will display basic information about the system's hostname, such as the current hostname, static hostname, icon name, and chassis type. 

Some of the commonly used options with the "hostnamectl" command are:

- "set-hostname": This option is used to set the system's hostname. For example, running "sudo hostnamectl set-hostname myhostname" will set the hostname to "myhostname". To make this change persistent across reboots, one would also need to update the "/etc/hostname" file with the new hostname.

- "status": This option provides detailed information about the system's hostname, including transient hostname, static hostname, and pretty hostname.

- "help": This option displays the help page for the "hostnamectl" command.

Overall, the "hostnamectl" command is a useful tool for managing the system's hostname in Linux-based systems. 

## tldr 
 
> Get or set the hostname of the computer.
> More information: <https://manned.org/hostnamectl>.

- Get the hostname of the computer:

`hostnamectl`

- Set the hostname of the computer:

`sudo hostnamectl set-hostname "{{hostname}}"`

- Set a pretty hostname for the computer:

`sudo hostnamectl set-hostname --static "{{hostname.example.com}}" && sudo hostnamectl set-hostname --pretty "{{hostname}}"`

- Reset hostname to its default value:

`sudo hostnamectl set-hostname --pretty ""`
