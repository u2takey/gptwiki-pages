# disown 
## chatgpt 
The "disown" command is a shell builtin that allows you to remove jobs from the shell's job control. When you run a command or start a process in a terminal, it becomes a job that is managed by the shell. You can see the list of jobs by typing "jobs" in the terminal.

However, when you quit the terminal or log out of the system, all the jobs associated with that terminal will be terminated. This can be a problem if you have a long-running process that you want to keep running even after you log out.

The "disown" command allows you to remove the job from the shell's control so that it continues running even after you close the terminal. To use the command, you first need to start a process or job in the terminal. Once the job is running, you can use the "disown" command with the job ID to remove it from the shell's job control.

The syntax of the "disown" command is as follows:

disown [-ar] [jobspec ...]

The "-a" option tells the shell to disown all jobs. The "-r" option tells the shell to remove the job from the job control and mark it as running even if it's stopped. The job specification can be a job ID or a job name. If no jobspec is given, the current job is used.

For example, to disown a job with job ID 1, you can run:

disown %1

This will remove the job from the shell's job control and mark it as running even if it's stopped. The job will continue running even after you close the terminal.

Note that the "disown" command only removes the job from the shell's job control. It does not make the job immune to signals or prevent it from accessing the terminal. If the job needs to interact with the terminal or receive signals, you may also need to redirect its input and output or use the "nohup" command. 

## tldr 
 
> Allow sub-processes to live beyond the shell that they are attached to.
> See also the `jobs` command.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#index-disown>.

- Disown the current job:

`disown`

- Disown a specific job:

`disown %{{job_number}}`

- Disown all jobs:

`disown -a`

- Keep job (do not disown it), but mark it so that no future SIGHUP is received on shell exit:

`disown -h %{{job_number}}`
