# stty 
## chatgpt 
The `stty` command is a utility for setting or printing terminal line settings. It is short for "set teletype". It is used to control various terminal line settings such as the speed of the connection, data bits, parity, flow control, and various other settings.

The syntax for `stty` command is:

```
stty options...
```

Some common options are:

- `-a`: displays all settings
- `-g`: displays current settings in a format that can be used as an argument to another `stty` command
- `-echo`: turns off echo
- `-icanon`: turns off canonical mode
- `sane`: sets all settings to default values

For example, to turn off echo and canonical mode, the command would be:

```
stty -echo -icanon
```

This command will make the terminal not echo back what you type, and will allow you to read input character-by-character instead of line-by-line. 

## tldr 
 
> Set options for a terminal device interface.
> More information: <https://www.gnu.org/software/coreutils/stty>.

- Display all settings for the current terminal:

`stty --all`

- Set the number of rows or columns:

`stty {{rows|cols}} {{count}}`

- Get the actual transfer speed of a device:

`stty --file {{path/to/device_file}} speed`

- Reset all modes to reasonable values for the current terminal:

`stty sane`
