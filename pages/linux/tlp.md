# tlp 
## chatgpt 
TLP is a command line tool that is used for power management on Linux systems. It helps to optimize the power consumption of laptops and other portable devices running on Linux by adjusting various power-related settings. TLP can be used to manage battery life, thermal management, and other power-related issues.

To use the TLP command, you need to have it installed on your Linux system. Once installed, you can open the terminal and type "tlp" followed by the appropriate parameters and options to perform specific tasks.

Some of the parameters and options that can be used with the TLP command include:

- '-h' or '--help': Displays a help message and a list of available options.
- '-s' or '--status': Displays the current status of TLP and its configuration settings.
- '-r' or '--reload': Reloads the TLP configuration file and applies any changes made to it.
- '-e' or '--enable': Enables TLP and applies its configuration settings.
- '-d' or '--disable': Disables TLP and restores the default power management settings.

Overall, the TLP command is a useful tool for managing power consumption on Linux systems, especially for laptops and other portable devices where battery life is a critical aspect of performance. 

## tldr 
 
> Advanced power management for Linux.
> See also `tlp-stat`.
> More information: <https://linrunner.de/tlp/>.

- Apply settings (according to the actual power source):

`sudo tlp start`

- Apply battery settings (ignoring the actual power source):

`sudo tlp bat`

- Apply AC settings (ignoring the actual power source):

`sudo tlp ac`
