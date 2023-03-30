# cpulimit 
## chatgpt 
cpulimit is a Linux command that allows you to limit the CPU usage of a process. It restricts the CPU usage of a process by temporarily pausing the execution of the process so that other processes can utilize the CPU resources. 

The cpulimit command works by sending signals to the process. When you run the command, it takes two arguments: the first argument is the maximum percentage of CPU usage that you want to allow, and the second argument is the process ID (PID) of the process that you want to limit.

For example, if you want to limit the CPU usage of a process with PID 1234 to 50%, you would use the following command:

cpulimit -p 1234 -l 50

The -p flag specifies the PID of the process that you want to limit, and the -l flag specifies the percentage of CPU usage that you want to allow.

Once you run the command, cpulimit will start monitoring the process and pause its execution if it starts using too much CPU. The duration and frequency of these pauses depends on the load of the system and the intensity of the workload of the process.

The cpulimit command can be useful in situations where you need to run multiple processor-intensive tasks simultaneously without overloading the CPU. It can also be used in situations where a process is using up all of the CPU resources and causing the system to slow down. With cpulimit, you can ensure that the offending process does not consume all the CPU resources and that other processes can run smoothly. 

## tldr 
 
> A tool to throttle the CPU usage of other processes.
> More information: <http://cpulimit.sourceforge.net/>.

- Limit an existing process with PID 1234 to only use 25% of the CPU:

`cpulimit --pid {{1234}} --limit {{25%}}`

- Limit an existing program by its executable name:

`cpulimit --exe {{program}} --limit {{25}}`

- Launch a given program and limit it to only use 50% of the CPU:

`cpulimit --limit {{50}} -- {{program arg1 arg2 ...}}`

- Launch a program, limit its CPU usage to 50% and run cpulimit in the background:

`cpulimit --limit {{50}} --background -- {{program}}`

- Kill its process if the program's CPU usage goes over 50%:

`cpulimit --limit 50 --kill -- {{program}}`

- Throttle both it and its child processes so that none go about 25% CPU:

`cpulimit --limit {{25}} --monitor-forks -- {{program}}`
