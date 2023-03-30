# srun 
## chatgpt 
`Srun` is a command that is used in a job submission script for the SLURM job scheduler system. It is used to launch a parallel job or a single job in a given number of nodes with the specified number of processes per node, within a time limit.

SLURM is a workload manager that is designed for high-performance computing clusters. It schedules and manages the allocation of resources and jobs on a cluster. Srun is one of the commands used in the SLURM job submission script, other commands include squeue, sbatch, scancel, and more.

When a user submits a job script, the srun command is used to start the job. It specifies the number of nodes and the number of processors per node. For instance, if a user wants to execute a parallel program on a cluster with 20 nodes and each node has 4 processors, the srun command would start the job as follows:

srun -N 20 -n 80 ./my_program

This command means that srun will start the job on 20 nodes, with a total of 80 processes. The "./my_program" tells srun to execute the code using each process.

Srun has a number of options that are used to customize the launch and execution of the job. For instance, srun can be used to specify the time limit for job execution, set the output file name, allocate memory, set environment variables, and more.

Overall, the srun command is a very useful tool for launching jobs and executing parallel programs in the SLURM job scheduler system. 

## tldr 
 
> Create an interactive slurm job or connect to an existing job.
> More information: <https://slurm.schedmd.com/srun.html>.

- Submit a basic interactive job:

`srun --pty /bin/bash`

- Submit an interactive job with different attributes:

`srun --ntasks-per-node={{num_cores}} --mem-per-cpu={{memory_MB}} --pty /bin/bash`

- Connect to a worker node with a job running:

`srun --jobid={{job_id}} --pty /bin/bash`
