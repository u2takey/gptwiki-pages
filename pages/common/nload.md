# nload 
## chatgpt 
The "nload" command is a type of network monitoring tool that allows you to view the amount of incoming and outgoing traffic on your network interface(s). Here's a breakdown of what the command does and how to use it:

Syntax:
nload [-h] [-V] [-i interval] [-m maxscale] [-o sides] [-a color] [-b color] [-t color] [-u unit] [-p priority] [-s size] [-X value] [-nd] [[-d device] [[-f filter expression][...]]]

Options:
-h — displays the help section for the command
-V — displays the version of the command
-i — specifies the update interval in seconds (default is 1 second)
-m — specifies the maximum scaling factor
-o — configures the output sides for the interface load graph (default is left and right)
-a — sets the color for the average value line
-b — sets the color for the background
-t — sets the color for the text
-u — sets the unit to display (default is bytes)
-p — specifies the priority level for the program
-s — sets the font size for the display
-X — overrides the default maximum value

Usage:
To use the "nload" command, simply enter the command followed by any relevant options and the name of the network interface you want to monitor. For example, to monitor the "eth0" interface, you would enter:

nload eth0

This will display a real-time graph of the incoming and outgoing traffic on that interface. You can use the arrow keys to navigate to different parts of the interface and keyboard shortcuts to configure different settings or options. Press "q" to exit the program.

Overall, "nload" is a useful tool for monitoring network traffic and identifying potential bottlenecks or issues with your connections. 

## tldr 
 
> A tool for visualizing network usage in the terminal.
> More information: <https://github.com/rolandriegel/nload>.

- View all network traffic (use the arrow keys to switch interfaces):

`nload`

- View network traffic on specific interfaces (use the arrow keys to switch interfaces):

`nload device {{interface_one}} {{interface_two}}`
