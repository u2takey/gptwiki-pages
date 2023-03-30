# gops 
## chatgpt 
gops is a command-line tool that provides a process explorer for Go. It allows you to interactively explore and monitor running Go programs.

When you run the "gops" command, it launches a process explorer in the terminal, displaying a list of all running Go processes on the system. You can select a process to view detailed information such as the process ID, command-line parameters, number of goroutines, heap and stack memory usage, and more.

You can also use gops to send signals to the selected process, such as triggering garbage collection, stopping or resuming the process, or profiling it with pprof. Additionally, gops can be used to create heap and goroutine dump files for further analysis.

Overall, gops is a useful tool for debugging and monitoring Go programs in real-time, providing valuable insights into their runtime behavior. 

## tldr 
 
> CLI tool which lists and diagnoses Go processes currently running on your system.
> More information: <https://github.com/google/gops>.

- Print all go processes running locally:

`gops`

- Print more information about a process:

`gops {{pid}}`

- Display a process tree:

`gops tree`

- Print the current stack trace from a target program:

`gops stack {{pid|addr}}`

- Print the current runtime memory statistics:

`gops memstats {{pid|addr}}`
