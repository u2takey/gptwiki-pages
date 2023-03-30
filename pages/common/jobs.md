# jobs 
## chatgpt 
The `jobs` command is used to display a list of active and background processes in a shell session. When a process is put in the background by appending an `&` character to the command, it continues to run, but allows the user to continue using the shell to execute other commands.

When the `jobs` command is executed, the shell displays the status of all active jobs, including their job number, status, and the command used to start them. The status column typically displays the words "running," "stopped," or "done" to indicate the current state of the job.

The `jobs` command can also be used with different options to selectively filter out specific jobs based on their status or other criteria. For example, the `-l` option can be used to display more detailed information about each job, including the process ID (PID) and the time at which the job was started.

Overall, the `jobs` command is a useful tool for managing and monitoring background processes in a shell environment, and can be especially helpful when working with complex or long-running tasks. 

## tldr 
 
> Display status of jobs in the current session.
> More information: <https://manned.org/jobs>.

- Show status of all jobs:

`jobs`

- Show status of a particular job:

`jobs %{{job_id}}`

- Show status and process IDs of all jobs:

`jobs -l`

- Show process IDs of all jobs:

`jobs -p`
