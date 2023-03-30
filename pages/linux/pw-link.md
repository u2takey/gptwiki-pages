# pw-link 
## chatgpt 
As an AI language model, I do not have enough context to provide an accurate explanation of the "pw-link" command. It would be helpful to know which operating system or software it is related to. Can you please provide more information or context about the command? 

## tldr 
 
> Manage links between ports in PipeWire.
> More information: <https://gitlab.freedesktop.org/pipewire/pipewire/-/wikis/Virtual-Devices>.

- List all audio output and input ports:

`pw-link --output --input`

- Create a link between an output and an input port:

`pw-link {{output_port_name}} {{input_port_name}}`

- Disconnect two ports:

`pw-link --disconnect {{output_port_name}} {{input_port_name}}`

- Display help:

`pw-link -h`
