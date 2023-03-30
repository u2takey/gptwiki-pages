# sstat 
## chatgpt 
As an AI language model, I don't have access to the context where you encountered the command "sstat" but typically: 

The command "sstat" is a system monitoring program in the Slurm workload manager. It is used to display detailed information about running and completed jobs, partitions, nodes, and clusters.

Some of the useful options of the sstat command are:

- `-j <job-id>`: This option allows you to specify the job ID of a particular job for which you want to display the details.

- `-u <user-id>`: This option allows you to specify the user ID of a particular user whose jobs you want to view.

- `-p <partition-name>`: This option allows you to specify the partition name for which you want to display details.

- `-S <start-time> -E <end-time>`: This option allows you to specify the start and end time window for which you want to display the job details.

- `-M <metric>`: This option allows you to specify the metric that you want the sstat command to display. Some of the metrics include CPU usage, memory usage, disk usage, etc.

- `-a`: This option displays all the available information about the specified job, partition, or node.

Overall, the sstat command is an essential tool for system administrators, developers, and high-performance computing users to monitor and manage their system resources. 

## tldr 
 
> View information about running jobs.
> More information: <https://slurm.schedmd.com/sstat.html>.

- Display status information of a comma-separated list of jobs:

`sstat --jobs={{job_id}}`

- Display job ID, average CPU and average virtual memory size of a comma-separated list of jobs, with pipes as column delimiters:

`sstat --parsable --jobs={{job_id}} --format={{JobID}},{{AveCPU}},{{AveVMSize}}`

- Display list of fields available:

`sstat --helpformat`
