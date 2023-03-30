# conky 
## chatgpt 
Conky is a command that is used to start the Conky system monitor. Conky is a light-weight system monitor tool for Linux that displays system information such as CPU usage, disk usage, RAM usage, network activity, and more on the desktop. 

The Conky command is used to start the system monitor and configure its display settings. The command typically includes various flags that specify what information is displayed and how it is presented. 

Here are some common flags used with the Conky command:

- -b : Runs Conky in the background.
- -c : Specifies the path to the Conky configuration file. 
- -d : Specifies the delay in seconds between updates.
- -i : Displays the PID of the running instance of Conky.
- -p : Specifies a custom port number for Conky to listen on for incoming connections.
- -q : Runs Conky in quiet mode, suppressing warning messages.
- -u : Displays CPU usage.
- -h : Displays help information about the available Conky flags.

Once Conky is running, it will display the specified system information on the desktop in real-time. Users can configure the display settings to customize the appearance and behavior of the system monitor. 

## tldr 
 
> Light-weight system monitor for X.
> More information: <https://github.com/brndnmtthws/conky>.

- Launch with default, built-in config:

`conky`

- Create a new default config:

`conky -C > ~/.conkyrc`

- Launch Conky with a given config file:

`conky -c {{path/to/config}}`

- Start in the background (daemonize):

`conky -d`

- Align Conky on the desktop:

`conky -a {{top|bottom|middle}}_{{left|right|middle}}`

- Pause for 5 seconds at startup before launching:

`conky -p {{5}}`
