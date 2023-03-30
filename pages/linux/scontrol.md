# scontrol 
## chatgpt 
scontrol is a command-line tool used for managing and viewing information related to Slurm workload manager. Slurm is a highly scalable, open-source workload manager used for managing and scheduling jobs on HPC (High-Performance Computing) clusters.

The scontrol command is used to interact with the Slurm controller daemon (slurmctld) and can perform various operations like submitting and monitoring jobs, querying cluster state, setting up node properties or job priorities, etc.

Some common scontrol usages are:

1. scontrol show: This command is used to display various Slurm resources and their current usage. For example, scontrol show node will show information about all nodes in the cluster, including their state, available resources, and load.

2. scontrol update: This command is used to update various parameters of Slurm resources. For example, scontrol update node=node01 state=down will set the state of node01 to down, effectively disabling it for job submission.

3. scontrol create: This command is used to create various Slurm resources like accounts, partitions, etc.

4. scontrol hold/release: These commands are used to place a job on hold or release it for execution, respectively.

Overall, scontrol provides a convenient and powerful interface for interacting with the Slurm workload manager. 

## tldr 
 
> View information about and modify jobs.
> More information: <https://slurm.schedmd.com/scontrol.html>.

- Show information for job:

`scontrol show job {{job_id}}`

- Suspend a comma-separated list of running jobs:

`scontrol suspend {{job_id}}`

- Resume a comma-separated list of suspended jobs:

`scontrol resume {{job_id}}`

- Hold a comma-separated list of queued jobs (Use `release` command to permit the jobs to be scheduled):

`scontrol hold {{job_id}}`

- Release a comma-separated list of suspended job:

`scontrol release {{job_id}}`
