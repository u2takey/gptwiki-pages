# sbatch 
## chatgpt 
The `sbatch` command is used in computing systems that utilize a job scheduler such as Slurm to submit a batch job to the cluster. The syntax of the command is typically as follows:

```sbatch [OPTIONS] [SBATCH_SCRIPT]```

The `[OPTIONS]` segment of the command allows for the specification of various options and flags to control the behavior of the job submission. Some commonly used options include:

- `--job-name=JOB_NAME` - Specifies the name of the job.
- `--time=TIME_LIMIT` - Specifies the maximum time that the job is allowed to run for.
- `--mem=MEMORY_LIMIT` - Specifies the amount of memory that the job requires.
- `--ntasks=NUM_TASKS` - Specifies the number of tasks that the job requires.
- `--cpus-per-task=CPUS_PER_TASK` - Specifies the number of CPUs that each task requires.

The `[SBATCH_SCRIPT]` segment of the command specifies the script that will be executed as the batch job. This script can be written in any programming language that is supported by the cluster, such as bash, Python, or R.

Once the `sbatch` command is executed, it submits the batch job to the cluster's job scheduler. The scheduler assigns the job to an available compute node, and the script specified in `[SBATCH_SCRIPT]` is executed on that node. The output of the script is typically written to a file specified by the user, which can be accessed once the job has completed. 

## tldr 
 
> Submit a batch job to the SLURM scheduler.
> More information: <https://manned.org/sbatch>.

- Submit a batch job:

`sbatch {{path/to/job.sh}}`

- Submit a batch job with a custom name:

`sbatch --job-name={{myjob}} {{path/to/job.sh}}`

- Submit a batch job with a time limit of 30 minutes:

`sbatch --time={{00:30:00}} {{path/to/job.sh}}`

- Submit a job and request multiple nodes:

`sbatch --nodes={{3}} {{path/to/job.sh}}`
