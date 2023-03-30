# autorandr 
## chatgpt 
The `autorandr` command is a utility used for managing display profiles on Linux systems. It is specifically designed to automatically detect and apply the appropriate display settings based on the connected hardware.

When the command is executed, it scans the system to detect available monitors and their properties, such as resolution, refresh rate, orientation, and position. It then checks if any predefined profiles match the detected configurations and applies the appropriate settings. If a matching profile is not found, `autorandr` creates a new profile based on the current display configuration.

The profiles created by `autorandr` can be easily managed and customized using configuration files. Users can define different profiles for different scenarios, such as home, office, or presentation mode.

Overall, `autorandr` simplifies the process of managing display settings on Linux systems, automating the task of switching between different display configurations manually. 

## tldr 
 
> Automatically change screen layout.
> More information: <https://github.com/phillipberndt/autorandr>.

- Save the current screen layout:

`autorandr --save {{profile_name}}`

- Show the saved profiles:

`autorandr`

- Load the first detected profile:

`autorandr --change`

- Load a specific profile:

`autorandr --load {{profile_name}}`

- Set the default profile:

`autorandr --default {{profile_name}}`
