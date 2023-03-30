# squeue 
## chatgpt 
The `squeue` command is a Linux command-line utility that is used to display the status of jobs that are currently running, in queue or recently completed on a High-Performance Computing (HPC) cluster.

When executed, the `squeue` command returns a list of jobs in a tabular format with the following columns:

- Job ID (JOBID): The unique identifier for the job.
- Partition (PARTITION): The partition or queue on which the job is running or scheduled to run.
- Name (NAME): The name of the job as specified by the user.
- User (USER): The username of the user who submitted the job.
- State (ST): The current state of the job, which can be PENDING, RUNNING, SUSPENDED, COMPLETING or CANCELLED.
- Time (TIME): The time for which the job has been running or scheduled to run.
- Nodes (NODES): The number of nodes allocated to the job.
- Reason (REASON): The reason for the job's current state, such as the time limit or dependency failure.

The `squeue` command can be executed with various options and arguments to filter the output according to specific requirements. For example, the `-u` option followed by a username can be used to display only the jobs submitted by that particular user, or the `-t` option followed by a job state can be used to display only the jobs in that particular state.

In summary, the `squeue` command provides a convenient way to monitor the status of jobs on an HPC cluster, helping users to track their own jobs and system administrators to manage the workload effectively. 

## tldr 
 
> View the jobs queued in the SLURM scheduler.
> More information: <https://manned.org/squeue>.

- View the queue:

`squeue`

- View jobs queued by a specific user:

`squeue -u {{username}}`

- View the queue and refresh every 5 seconds:

`squeue -i {{5}}`

- View the queue with expected start times:

`squeue --start`
