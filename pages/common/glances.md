# glances 
## chatgpt 
glances is a command-line system monitoring tool that provides real-time performance metrics about CPU usage, memory usage, disk I/O, network I/O, and other system parameters. The tool is written in Python and is compatible with Linux, FreeBSD, and macOS operating systems. Glances is an open-source project licensed under GPL v3.

When executed, the glances command will produce a console-based user interface that displays system performance data in a tabular format. The data is presented in a color-coded scheme making it easy to quickly identify any issues.

Some of the key metrics displayed by glances include:

- CPU usage: displays CPU utilization by each core, as well as system-wide utilization.
- Memory usage: shows the memory utilization of each process on the system.
- Network usage: displays incoming and outgoing network traffic.
- Disk I/O: provides information on disk utilization and the amount of data being read and written.
- Process details: shows detailed information about every process running on the system.

Additionally, glances provides the ability to customize the interface, add alarms to notify when certain thresholds are met, and export data to external systems.

Overall, glances is a powerful tool that offers a comprehensive view of system performance data, making it an ideal solution for system administrators and developers. 

## tldr 
 
> A cross-platform system monitoring tool.
> More information: <https://nicolargo.github.io/glances/>.

- Run in terminal:

`glances`

- Run in web server mode to show results in browser:

`glances -w`

- Run in server mode to allow connections from other Glances clients:

`glances -s`

- Connect to a Glances server:

`glances -c {{hostname}}`

- Require a password in (web) server mode:

`glances -s --password`
