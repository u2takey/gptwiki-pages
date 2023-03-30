# sensors 
## chatgpt 
The command "sensors" is a Linux command that is used to display the system's temperature measurements of various components such as CPU, GPU, motherboard, hard disk, etc. The sensors command is used to monitor the temperatures of hardware components in real-time. It provides a command-line interface to get the temperature readings of various sensors installed in the system.

When issued, this command will collect data from the system's sensors and display the readings in the terminal window. The output typically contains a list of sensors along with their corresponding temperature readings. The temperature readings are displayed in degrees Celsius or Fahrenheit, depending on the user's preferred unit of measurement.

The information provided by the "sensors" command helps users to monitor the system's temperature and avoid overheating or hardware failure. It is especially useful for users who run resource-intensive applications or those who overclock their hardware components. Additionally, it can help troubleshoot issues related to thermal throttling, heating, and cooling. 

In order to use the "sensors" command, the lm-sensors package must be installed on the system. This can be done using the package manager of the respective Linux distribution. Once the package is installed, the command can be used to access temperature data. 

## tldr 
 
> Report sensors information.
> More information: <https://manned.org/sensors>.

- Show the current readings of all sensor chips:

`sensors`

- Show temperatures in degrees Fahrenheit:

`sensors --fahrenheit`
