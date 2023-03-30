# wait 
## chatgpt 
The wait command is used to pause the execution of a shell script until a background process or job is finished. 

Syntax:
```
wait [pid ...]
```
where, pid is the process ID of the job or process that needs to be waited for. If no PID is specified, the command waits for all currently pending background jobs to finish. 

Once the specified process or all background jobs are finished, the script execution resumes.

Example:
```
#!/bin/bash
echo "Starting a long running process..."
sleep 10 &
wait $!
echo "Long running process finished."
```
In the above example, the `sleep 10` command runs in the background and the script waits for it to finish using the `wait` command with `$!` as the argument. `$!` is a special shell variable that contains the PID of the last background process. Once the `sleep 10` command is finished, the script resumes and the message "Long running process finished." is printed to the console.

Note: The wait command can only be used within a shell script and not on the command line. 

## tldr 
 
> Wait for a process to complete before proceeding.
> More information: <https://manned.org/wait>.

- Wait for a process to finish given its process ID (PID) and return its exit status:

`wait {{pid}}`

- Wait for all processes known to the invoking shell to finish:

`wait`
