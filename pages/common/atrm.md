# atrm 
## chatgpt 
The atrm command is a Unix/Linux command used to remove jobs from the at queue. The at queue is a scheduler in Unix/Linux that is used to execute commands or scripts at a specified time or date. The atrm command is used to remove or delete jobs that have been scheduled in the at queue.

The syntax of the atrm command is as follows:

atrm [job ID]

where [job ID] is the ID number of the job that you want to remove or delete. You can use the 'atq' command to see the list of jobs in the at queue and their corresponding job IDs.

When you run the atrm command with a valid job ID, it will remove the job from the at queue and delete it from the system. If you run the command with an invalid job ID or no job ID, it will display an error message.

It's important to note that when you remove a job from the at queue using the atrm command, it will not be executed. If you want to reschedule the job for a different time, you will need to create a new job using the 'at' command. 

## tldr 
 
> Remove jobs scheduled by `at` or `batch` commands.
> To find job numbers use `atq`.
> More information: <https://manned.org/atrm>.

- Remove job number 10:

`atrm {{10}}`

- Remove many jobs, separated by spaces:

`atrm {{15}} {{17}} {{22}}`
