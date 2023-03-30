# jobs 
## chatgpt 
The "jobs" command is used in Unix and Unix-like operating systems to display a list of jobs that are running in the background. The jobs command is primarily used in two use cases:

1. To display all of the jobs associated with the current terminal.

2. To display all of the jobs that are currently running in the system, regardless of the terminal with which they are associated.

When the jobs command is executed, it displays the job number, state, and name or command that was executed. The job number is a unique identifier assigned to each job when it is created. The state of the job can be one of the following:

1. Running - The job is currently running in the background.

2. Stopped - The job has been stopped or paused by the user or the system.

3. Terminated - The job has completed or has been terminated by the user or the system.

Additionally, the jobs command can be used with various options to modify its behavior. For example, the "jobs -l" command will display additional information about the jobs, such as the PID (process ID) of the job and the terminal that it is associated with. The "jobs -n" command will display only jobs that have changed status since the last time the jobs command was executed. 

Overall, the jobs command is a powerful tool for monitoring and managing background jobs on Unix systems. 

## tldr 
 
> BASH builtin for viewing information about processes spawned by the current shell.
> More information: <https://manned.org/jobs>.

- View jobs spawned by the current shell:

`jobs`

- List jobs and their process IDs:

`jobs -l`

- Display information about jobs with changed status:

`jobs -n`

- Display process ID of process group leader:

`jobs -p`

- Display running processes:

`jobs -r`

- Display stopped processes:

`jobs -s`
