# lpinfo 
## chatgpt 
The "lpinfo" command is used to gather information about available printers and printer drivers on a Linux system.

When used without any parameters or options, lpinfo outputs a list of all printers defined on the system, including their names, supported page sizes, and the printer driver used by each. It also shows the connection type for each printer (such as USB, network, or parallel) and the device URI or network address used to communicate with the printer.

Some of the common options for the lpinfo command are:

- -m or --make-and-model: This option lists the available printer drivers and their corresponding make and model names.
- -v or --device-uri: This option shows the device URI for each printer, which can be used to configure the printer in CUPS or other printing software.
- -h or --help: This option displays the help message and available options for the lpinfo command.

Overall, the lpinfo command is a useful tool for inspecting the printing system on a Linux machine and providing details about available printers and their driver configurations. 

## tldr 
 
> List connected printers and installed drivers for the CUPS print server.
> More information: <https://www.cups.org/doc/man-lpinfo.html>.

- List all the currently connected printers:

`lpinfo -v`

- List all the currently installed printer drivers:

`lpinfo -m`

- Search installed printer drivers by make and model:

`lpinfo --make-and-model "{{printer_model}}" -m`
