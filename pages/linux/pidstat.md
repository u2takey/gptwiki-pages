# pidstat 
## chatgpt 
pidstat is a command used in Linux to display detailed statistics on processor usage and other critical resources being used by a given process. It provides a real-time view of CPU utilization statistics for each running process, threads, or specific process IDs specified.

Syntax: 

`pidstat [options] [interval] [count]`

Here, options are the additional parameters that can be used to customize the output produced by pidstat.

Interval represents the time to wait in seconds between each report.

Count indicates the number of reports to print, after which pidstat will exit automatically.

Some commonly used options:

* `-u`: This option displays information about the utilization of the CPU processors.

* `-p`: It allows you to specify a comma-separated list of process IDs (PIDs) for monitoring.

* `-r`: Provides specific memory utilization statistics, such as page faults.

* `-d`: Shows the statistics related to block device input and output operations.

* `-t`: Provides a breakdown of the statistics per thread within the process ID.

* `-h`: This option prints the help screen and command syntax.

By default, pidstat displays CPU and memory usage statistics with a one-second interval and no limit on the number of reports to print. This command can be useful in troubleshooting performance issues in a Linux environment by identifying processes that consume too many resources. 

## tldr 
 
> Show system resource usage, including CPU, memory, IO etc.
> More information: <https://manned.org/pidstat>.

- Show CPU statistics at a 2 second interval for 10 times:

`pidstat {{2}} {{10}}`

- Show page faults and memory utilization:

`pidstat -r`

- Show input/output usage per process id:

`pidstat -d`

- Show information on a specific PID:

`pidstat -p {{PID}}`

- Show memory statistics for all processes whose command name include "fox" or "bird":

`pidstat -C "{{fox|bird}}" -r -p ALL`
