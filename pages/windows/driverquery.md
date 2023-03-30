# driverquery 
## chatgpt 
The driverquery command is a Windows command that retrieves a list of all installed device drivers and their properties. It displays information such as driver name, type, status, start mode, manufacturer, and version number. This information can be useful for diagnosing problems with devices and finding the most up-to-date drivers.

The syntax for the driverquery command is as follows:

driverquery [/FO format] [/NH] [/SI] [/V]

- /FO format: specifies the output format, which can be table, list, CSV, or HTML.
- /NH: omits the column headers from the output.
- /SI: displays the digital signature information for each driver.
- /V: displays verbose information, including driver date and file size.

To use the driverquery command, open a Command Prompt window and type the command followed by any parameters. The output will be displayed in the window or in the specified format.

Example: driverquery /fo csv /v > drivers.csv

This command retrieves a list of drivers in CSV format and saves the output to a file called "drivers.csv" for further analysis. The "/v" option displays additional information about each driver. 

## tldr 
 
> Display information about installed device drivers.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/driverquery>.

- Display a list of all installed device drivers:

`driverquery`

- Display a list of drivers in the specified format:

`driverquery /fo {{table|list|csv}}`

- Display a list of drivers with a column to indicate if they are signed:

`driverquery /si`

- Exclude the header in the output list:

`driverquery /nh`

- Display a list of drivers for a remote machine:

`driverquery /s {{hostname}} /u {{username}} /p {{password}}`

- Display a list of drivers with verbose information:

`driverquery /v`

- Display detailed usage information:

`driverquery /?`
