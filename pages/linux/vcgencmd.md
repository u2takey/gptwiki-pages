# vcgencmd 
## chatgpt 
vcgencmd is a command-line tool provided by the Raspberry Pi Foundation for interacting with the Videocore GPU on the Raspberry Pi. This tool allows you to get information about the GPU and configure various settings.

The vcgencmd tool provides several sub-commands that allow you to do things like:

- get the temperature of the GPU
- get the frequency of the GPU and other system components
- get the amount of memory allocated to the GPU
- get information about the HDMI output
- over- or underclock the GPU
- enable or disable various features

Here are some examples of how to use the vcgencmd tool:

- To get the temperature of the GPU, run: `vcgencmd measure_temp`. This will output something like: `temp=54.5'C`
- To get the frequency of the GPU, run: `vcgencmd measure_clock arm`. This will output something like: `frequency(45)=1200000000`
- To get the amount of memory allocated to the GPU, run: `vcgencmd get_mem arm`. This will output something like: `arm=960M`
- To get information about the HDMI output, run: `vcgencmd get_config int`. This will output a list of parameters, including things like `hdmi_force_hotplug` and `hdmi_group`.
- To over- or underclock the GPU, run: `vcgencmd measure_clock arm <frequency>`. For example, to overclock the GPU to 1.5 GHz, run: `vcgencmd measure_clock arm 1500000000`.
- To enable or disable features, use the `get_config` and `set_config` sub-commands. For example, to disable the camera module, run: `vcgencmd set_config disable_camera_led 1`.

Keep in mind that some features may require sudo access or changes to the boot configuration in order to take effect. Always be careful when making changes with the vcgencmd tool, as incorrect settings can cause instability or damage to your Raspberry Pi. 

## tldr 
 
> Print system information for a Raspberry Pi.
> More information: <https://www.raspberrypi.org/documentation/computers/os.html#vcgencmd>.

- List all available commands:

`vcgencmd commands`

- Print the current CPU temperature:

`vcgencmd measure_temp`

- Print the current voltage:

`vcgencmd measure_volts`

- Print the throttled state of the system as a bit pattern:

`vcgencmd get_throttled`

- Print the bootloader config (only available on Raspberry Pi 4 models):

`vcgencmd bootloader_config`

- Display Help:

`vcgencmd --help`
