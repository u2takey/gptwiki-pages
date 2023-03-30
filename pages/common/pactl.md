# pactl 
## chatgpt 
pactl stands for PulseAudio Control. It is a command-line utility tool that is used to control and configure the PulseAudio sound server on Linux systems.

The pactl command allows you to monitor and control the sound volume, mute or unmute audio devices, load or unload modules, list and manage sinks and sources, set up loopbacks for audio routing, and many other audio-related tasks.

Some of the commonly used options of the pactl command are:

- pactl list: This option lists all the available sinks, sources, and modules currently loaded by PulseAudio.
- pactl set-sink-volume: This option is used to set the volume of a particular sink (speaker or headphone) to a specified value.
- pactl set-source-mute: This option can be used to mute or unmute a particular source (microphone or line-in).
- pactl load-module: This option loads a new module into the PulseAudio server. Modules can be sound processing units, audio filters, or devices.
- pactl unload-module: This option unloads a previously loaded module from the PulseAudio server.

Overall, pactl is a very useful command-line utility tool for controlling and troubleshooting audio-related issues on Linux systems. 

## tldr 
 
> Control a running PulseAudio sound server.
> More information: <https://manned.org/pactl>.

- List all sinks (or other types - sinks are outputs and sink-inputs are active audio streams):

`pactl list {{sinks}} short`

- Change the default sink (output) to 1 (the number can be retrieved via the `list` subcommand):

`pactl set-default-sink {{1}}`

- Move sink-input 627 to sink 1:

`pactl move-sink-input {{627}} {{1}}`

- Set the volume of sink 1 to 75%:

`pactl set-sink-volume {{1}} {{0.75}}`

- Toggle mute on the default sink (using the special name `@DEFAULT_SINK@`):

`pactl set-sink-mute {{@DEFAULT_SINK@}} toggle`
