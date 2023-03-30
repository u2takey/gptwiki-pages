# perf 
## chatgpt 
"perf" is a performance monitoring tool available in Linux-based operating systems. It is used to measure various system events such as CPU instructions executed per second, cache misses, and context switches. "perf" allows developers and system administrators to understand and optimize the system's performance.

To use "perf," the user needs to install the "perf" package, which is available in most Linux distributions. Once installed, the user can run "perf" with various subcommands and options to monitor different events. Here are some of the commonly used subcommands and options:

- "perf record [command]" - This subcommand records the specified command's performance data, such as CPU cycles, cache misses, etc., and saves it to a file.
- "perf report [options]" - This subcommand displays the performance data recorded by the "perf record" subcommand in a human-readable format. The user can use various options to customize the output format and filter the data.
- "perf stat [options] [command]" - This subcommand runs the specified command and displays performance statistics, such as CPU cycles, cache misses, etc. The user can use various options to customize the output format and choose which events to track.

Overall, "perf" is a powerful tool for monitoring and optimizing a system's performance. It can help developers and system administrators identify bottlenecks and fine-tune the system's settings. However, it requires some knowledge and experience to use effectively. 

## tldr 
 
> Framework for Linux performance counter measurements.
> More information: <https://perf.wiki.kernel.org>.

- Display basic performance counter stats for a command:

`perf stat {{gcc hello.c}}`

- Display system-wide real-time performance counter profile:

`sudo perf top`

- Run a command and record its profile into `perf.data`:

`sudo perf record {{command}}`

- Record the profile of an existing process into `perf.data`:

`sudo perf record -p {{pid}}`

- Read `perf.data` (created by `perf record`) and display the profile:

`sudo perf report`
