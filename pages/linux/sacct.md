# sacct 
## chatgpt 
The "sacct" command is used to display and report details about jobs and tasks that have been run on the Slurm resource manager (a workload manager used on Linux clusters). 

Here are the details about the sacct command:

- By default, sacct will display a summary of all jobs that have been run on the cluster, including their job ID, user ID, job name, status, start and end times, and more.
- If you want to filter the output to show only specific jobs or tasks, you can use various command-line options, such as the "--job" option to filter by job ID, or the "--state" option to filter by job status. 
- You can also use sacct to generate reports in various formats, including CSV, HTML, and JSON. To do so, you would use the "--format" option to specify the output format, and the "--parsable" option to get machine-readable output.
- Other options for the sacct command include the ability to display details about completed jobs only, display details about running jobs only, show details about jobs that failed, show details about jobs that exceeded their time limits, and more. 

Overall, sacct is a powerful command that can provide valuable insights and reporting on job and task activity on a Slurm cluster, helping administrators to identify and address issues, optimize resource usage, and more. 

## tldr 
 
> Display accounting data from the Slurm service.
> More information: <https://slurm.schedmd.com/sacct.html>.

- Display job id, job name, partition, account, number of allocated cpus, job state, and job exit codes for recent jobs:

`sacct`

- Display job id, job state, job exit code for recent jobs:

`sacct --brief`

- Display the allocations of a job:

`sacct --jobs {{job_id}} --allocations`

- Display elapsed time, job name, number of requested CPUs, and memory requested of a job:

`sacct --jobs {{job_id}} --format={{elapsed}},{{jobname}},{{reqcpus}},{{reqmem}}`
