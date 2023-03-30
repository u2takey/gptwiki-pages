# screenfetch 
## chatgpt 
Screenfetch is a command-line utility that displays information about the user's operating system and hardware, as well as ASCII art depicting the logo of the user's distribution.

When the user enters the "screenfetch" command, the utility immediately begins collecting information from the system. This information includes the distribution name and version, kernel version, CPU information, memory usage, and graphics driver information, among others.

Once this information has been collected, screenfetch creates an ASCII art image of the distribution's logo, which is typically displayed at the top of the output. This is followed by the system information, displayed in a formatted and easy-to-read manner.

Screenfetch can be useful for quickly displaying important system information for troubleshooting, or just for showing off one's system specs to others. It is available for a wide variety of Linux distributions and can by installed using the package manager of the user's distribution. 

## tldr 
 
> Display system information.
> More information: <https://github.com/KittyKatt/screenFetch>.

- Start screenfetch:

`screenfetch`

- Take a screenshot (requires 'scrot'):

`screenfetch -s`

- Specify distribution logo:

`screenfetch -A '{{distribution_name}}'`

- Specify distribution logo and text:

`screenfetch -D '{{distribution_name}}'`

- Strip all color:

`screenfetch -N`
