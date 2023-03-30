# scancel 
## chatgpt 
The `scancel` command is used in Linux-based systems to cancel a running or queued job or task that was submitted to a Slurm job scheduler. Here are the details of the `scancel` command:

Syntax:
```
scancel [options] [jobid | jobid-range | jobname | jobname-range]
```

Options:
- `-h, --help`: Displays the help menu for `scancel`.
- `-V, --version`: Displays the version number of `scancel`.
- `-u, --user=username`: Cancels all jobs submitted by the specified user.
- `-t, --state=STATE`: Cancels all jobs in the specified state (e.g. PENDING, RUNNING, SUSPENDED, etc.).
- `-s, --signal=SIGNAL`: Sends the specified signal to the job instead of canceling it.
- `-c, --checkpoint`: Requests a checkpoint of the job before canceling it.
- `-n, --nodes=NODELIST`: Cancels all jobs running on the specified nodes.
- `-G, --set-gres`: Cancel all jobs with the specified generic resource assigned.
- `-g, --gres`: Cancel all jobs that explicitly request given generic resource.

Arguments:
- `jobid`: The job ID(s) to cancel. Multiple IDs can be specified separated by commas or in a range with a dash (e.g. `123,456-458`).
- `jobname`: The job name(s) to cancel. Multiple names can be specified separated by commas or in a range with a dash (e.g. `test_job,my_jobs-15`).

Note that `scancel` requires the user to have proper authorization to cancel a job. Cancelling a job can lead to unexpected behavior and should be used with caution. 

## tldr 
 
> Cancel a Slurm job.
> More information: <https://slurm.schedmd.com/scancel.html>.

- Cancel a job using its ID:

`scancel {{job_id}}`

- Cancel all jobs from a user:

`scancel {{user_name}}`
