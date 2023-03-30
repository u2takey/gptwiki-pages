# qsub 
## chatgpt 
The command "qsub" is a command used in high-performance computing clusters to submit batch jobs. It is usually used when there is a need to do a task on a remote cluster that requires significant computational resources. The qsub command allows users to submit a batch job to a queue system, which can efficiently manage the available resources.

Here is a detailed explanation of the command:

- The first thing to understand is that qsub is a command-line utility, which means it is used in a Unix-like terminal. Therefore, to use the command, one must open a terminal and type the command.

- The qsub command is followed by the name of the script file that contains the job that needs to be run on the remote cluster. The file can be a Bash, Perl, or Python script, among others. The script file usually contains directives that specify the required resources, such as the memory, number of cores, and the time needed to run the job.

- After submitting the job using the qsub command, the job enters a queue. Jobs are usually executed in the order they are received, although the scheduling policy can be configured to prioritize certain types of jobs or users.

- Once the job starts running, the output is redirected to a file specified in the script file. The output file contains the results of the job, such as log messages, errors, and other relevant information.

- One important feature of the qsub command is the ability to submit multiple jobs simultaneously using an array. In an array, a single script file is submitted with different input parameters, and each instance of the script runs with a different set of parameters.

In summary, qsub is a powerful command-line utility that allows users to submit batch jobs to high-performance computing clusters. It simplifies the management and scheduling of computational resources, and its features, such as arrays, make it versatile for running different types of jobs. 

## tldr 
 
> Submits a script to the queue management system TORQUE.
> More information: <https://manned.org/qsub.1>.

- Submit a script with default settings (depends on TORQUE settings):

`qsub {{script.sh}}`

- Submit a script with a specified wallclock runtime limit of 1 hour, 2 minutes and 3 seconds:

`qsub -l walltime={{1}}:{{2}}:{{3}} {{script.sh}}`

- Submit a script that is executed on 2 nodes using 4 cores per node:

`qsub -l nodes={{2}}:ppn={{4}} {{script.sh}}`

- Submit a script to a specific queue. Note that different queues can have different maximum and minimum runtime limits:

`qsub -q {{queue_name}} {{script.sh}}`
