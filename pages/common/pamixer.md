# pamixer 
## chatgpt 
Pamixer is a command-line interface tool for controlling PulseAudio sound server's mixer settings. PulseAudio is a sound server used in many modern Linux distributions to handle audio playback, mixing, and routing. 

The pamixer command can be used to control and adjust the volume levels of different playback devices and applications in the PulseAudio system. With pamixer, you can do things such as mute and unmute audio sources, adjust volume levels, change the active audio source, and more.

The basic syntax for using pamixer is:

pamixer [option] [value]

Here are some of the most commonly used options for pamixer:

- --list-sinks: Lists all the available sinks (output devices) in the system.

- --list-sources: Lists all the available sources (input devices) in the system.

- --sink-inputs: Lists all the applications playing audio, along with their corresponding ID numbers.

- --get-volume: Returns the current volume level. 

- --increase / --decrease: Increases or decreases the volume level by a specified value.

- --mute / --unmute: Mutes or unmutes the output.

For instance, to set the volume to 50%, you can use the following command:

pamixer --set-volume 50

Similarly, to mute the output, use:

pamixer --mute

Overall, pamixer is a useful tool for managing the sound settings of a Linux system, specifically the PulseAudio sound server. 

## tldr 
 
> A simple command-line mixer for PulseAudio.
> More information: <https://github.com/cdemoulins/pamixer>.

- List all sinks and sources with their corresponding IDs:

`pamixer --list-sinks --list-sources`

- Set the volume to 75% on the default sink:

`pamixer --set-volume {{75}}`

- Toggle mute on a sink other than the default:

`pamixer --toggle-mute --sink {{ID}}`

- Increase the volume on default sink by 5%:

`pamixer --increase {{5}}`

- Decrease the volume on a source by 5%:

`pamixer --decrease {{5}} --source {{ID}}`

- Use the allow boost option to increase, decrease, or set the volume above 100%:

`pamixer --set-volume {{105}} --allow-boost`

- Mute the default sink (use `--unmute` instead to unmute):

`pamixer --mute`
