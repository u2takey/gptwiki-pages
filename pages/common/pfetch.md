# pfetch 
## chatgpt 
pfetch is a command-line tool used for displaying system information on Linux and other Unix-like operating systems. Its name stands for "pretty fetch", which refers to the colorful ASCII art logo that is displayed along with the system information. Here's a breakdown of what the pfetch command does:

1. Displays System Information: When you run the pfetch command, it displays various information about your system, such as your operating system name and version, the kernel version, the CPU and GPU model, the system uptime, and the available memory, among others. This information is useful for system administrators and other users who need to know more about their systems' specifications.

2. Customizable: pfetch is highly customizable, and you can modify the output by adding or removing modules. By default, it displays several modules, including the OS logo, hostname, OS name and version, kernel version, CPU and GPU model, memory usage and uptime. You can use command-line switches to customize the output of pfetch.

3. ASCII Art Logo: The most distinctive feature of pfetch is its colorful ASCII art logo that appears at the top of the output. The logo depicts a small animal (e.g., a penguin or a cat) along with the name of the distribution that is being used. This makes the tool visually pleasing and adds an element of fun to the standard command-line interface.

4. Lightweight: pfetch is a lightweight tool that consumes minimal system resources, making it ideal for older systems or low-powered devices. It is written in the C programming language and has minimal dependencies, making it easy to install and run on almost any system.

Overall, pfetch is a useful and lightweight tool for displaying system information on Linux and other Unix-like operating systems. Its customizable output, colorful ASCII art logo, and lightweight design make it a popular choice among Linux users. 

## tldr 
 
> Display system information.
> More information: <https://github.com/dylanaraps/pfetch>.

- Display the ASCII art and default fields:

`pfetch`

- Display only the ASCII art and color palette fields:

`PF_INFO="{{ascii palette}}" pfetch`

- Display all possible fields:

`PF_INFO="{{ascii title os host kernel uptime pkgs memory shell editor wm de palette}}" pfetch`

- Display a different username and hostname:

`USER="{{user}}" HOSTNAME="{{hostname}}" pfetch`

- Display without colors:

`PF_COLOR={{0}} pfetch`
