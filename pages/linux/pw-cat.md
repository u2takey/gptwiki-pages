# pw-cat 
## chatgpt 
"pw-cat" is a command used in the Unix-like operating systems, such as Linux and macOS. The command is used to display the contents of a password file, which typically stores user login credentials and other authentication data.

The syntax of the command is:

pw-cat [options] [file]

The options available with the command are:

- -h or --help: Displays the help message for the command.
- -v or --version: Displays the version details of the command.

The "file" parameter specifies the path to the password file that you want to display.

When you execute the "pw-cat" command with the required parameters, it will read the contents of the specified password file and print them on the terminal screen. You can use this command to view the contents of important password files, such as "/etc/passwd" or "/etc/shadow". However, keep in mind that these files may be readable only by the root user, who has administrative privileges, due to security reasons. 

## tldr 
 
> Pipewire tool for playing and recording audio files.
> More information: <https://fedoraproject.org/wiki/QA:Testcase_PipeWire_PipeWire_CLI>.

- List all available playback targets:

`pw-cat --playback --list-targets`

- Play a WAV file over the default target:

`pw-cat --playback {{path/to/file.wav}}`

- List all available record targets:

`pw-cat --record --list-targets`

- Record a sample recording at a different volume level:

`pw-cat --record --volume={{0.1}} {{path/to/file.wav}}`

- Record a sample recording using a different sample rate:

`pw-cat --record --rate={{6000}} {{path/to/file.wav}}`
