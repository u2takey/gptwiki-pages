# py-spy 
## chatgpt 
Py-spy is a command-line tool used to profile Python programs in real-time without modifying the code. It can be used to extract detailed information about the performance and behaviour of your Python application, as well as identify where bottlenecks and performance issues are located.

When running the `py-spy` command, you need to specify the target Python process to be profiled by providing the process ID, or the name of the script file that is executing. The command will initiate the profiling process, and start collecting real-time data on the performance of the target Python program.

During the profiling, `py-spy` will capture information such as function call stack, CPU usage, memory usage, thread activity, and other performance metrics. The collected data is then presented in a clear and concise format, such as flame graphs and tables, which can be easily analyzed and interpreted.

Py-spy is a powerful tool for developers, system administrators, and performance testers who need to optimize the performance of their Python applications. It can help you identify issues early on, and improve the scalability and stability of your software. 

## tldr 
 
> A sampling profiler for Python programs.
> More information: <https://github.com/benfred/py-spy>.

- Show a live view of the functions that take the most execution time of a running process:

`py-spy top --pid {{pid}}`

- Start a program and show a live view of the functions that take the most execution time:

`py-spy top -- python {{path/to/file.py}}`

- Produce an SVG flame graph of the function call execution time:

`py-spy record -o {{path/to/profile.svg}} --pid {{pid}}`

- Dump the call stack of a running process:

`py-spy dump --pid {{pid}}`
