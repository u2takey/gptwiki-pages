# atq 
## chatgpt 
The command "atq" is used in Linux and Unix-based operating systems to display the list of pending jobs in the "at" queue. The "at" command is used to schedule a one-time task to run at a specified time and date.

The "atq" command lists all the jobs in the queue, including their ID number, scheduled time, and date. The output is similar to the following:

554   Wed Sep 15 12:14:00 2021 a user
555   Thu Sep 16 11:00:00 2021 a user
556   Fri Sep 17 09:30:00 2021 a user

In this example, there are three pending jobs in the queue. The ID number identifies the job, followed by the scheduled date and time. The last column shows the username of the person who scheduled the job.

You can use the "atrm" command to remove a job from the queue by specifying its ID number. For example, "atrm 554" will remove the first job in the queue with an ID of 554. 

## tldr 
 
> Show jobs scheduled by `at` or `batch` commands.
> More information: <https://manned.org/atq>.

- Show the current user's scheduled jobs:

`atq`

- Show jobs from queue named 'a' (queues have single-character names):

`atq -q {{a}}`

- Show jobs of all users (run as superuser):

`sudo atq`
