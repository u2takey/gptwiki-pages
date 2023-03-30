# cups-config 
## chatgpt 
cups-config is a command-line utility that is available in Unix-based operating systems, specifically designed for the Common Unix Printing System (CUPS).

When you run the "cups-config" command, it will display the configuration information of the CUPS print queue and the CUPS itself. Here are some of the most commonly used options with the cups-config command:

- --cflags: This option is used to get information regarding the compiler flags required to compile a CUPS application. It provides the location of CUPS headers and libraries.

- --help: This option displays the help information about the cups-config command.

- --libs: This option is used to print the library flags required to link with the CUPS library. It includes the location of the CUPS library.

- --serverbin: This option is used to locate the cupsd executable file.

- --serverroot: This option is used to locate the CUPS configuration directory where cupsd.conf and other configuration files are stored.

Overall, the cups-config command provides valuable information about the CUPS printing system and its configuration, helping you troubleshoot any printer-related issues or configure your printer setup more efficiently. 

## tldr 
 
> Show technical information about your CUPS print server installation.
> More information: <https://www.cups.org/doc/man-cups-config.html>.

- Show the currently installed version of CUPS:

`cups-config --version`

- Show where CUPS is currently installed:

`cups-config --serverbin`

- Show the location of CUPS' configuration directory:

`cups-config --serverroot`

- Show the location of CUPS' data directory:

`cups-config --datadir`

- Display all available options:

`cups-config --help`
