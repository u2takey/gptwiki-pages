# kscreen-doctor 
## chatgpt 
The command "kscreen-doctor" is a utility that is available on KDE (K Desktop Environment) based Linux distributions. It is used to diagnose and troubleshoot any issues related to display screens.

When the command is executed, it performs a diagnostic check of the display screens and outputs any found problems to the console. This diagnostic check includes checking for any misconfigured display settings such as resolution, refresh rate, and rotation. It also checks the connection between the computer and display device to ensure that it is properly connected and operating.

The output of the command provides detailed information about the detected problem, including suggested solutions. Based on this information, a user can make changes to the display settings or take necessary actions to resolve the issue.

In summary, "kscreen-doctor" is a helpful command for diagnosing and resolving display-related issues on KDE-based Linux systems. 

## tldr 
 
> Change and manipulate the screen setup from the command-line.
> More information: <https://invent.kde.org/plasma/libkscreen>.

- Show display output information:

`kscreen-doctor --outputs`

- Set the rotation of a display output with an ID of 1 to the right:

`kscreen-doctor {{output.1.rotation.right}}`

- Set the scale of a display output with an ID of `HDMI-2` to 2 (200%):

`kscreen-doctor {{output.HDMI-2.scale.2}}`
