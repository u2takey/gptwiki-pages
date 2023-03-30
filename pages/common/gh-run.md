# gh run 
## chatgpt 
The command "gh run" is a command-line interface (CLI) command used to create, view, and manage workflow runs within a GitHub repository. Here is a detailed explanation of the various aspects of this command:

- "gh": it refers to the GitHub CLI tool, which allows developers to interact with GitHub from the command line. It's an official CLI tool offered by GitHub.

- "run": it is a subcommand of the "gh" tool, used to initiate or view a workflow run.

Some of the common options used with the "gh run" command include:

- "list": It is used to list all the current or past workflow runs in the repository.

- "view": It is used to view the details of a specific workflow run. You can specify the run ID, the branch the run was triggered on, or the name of the workflow.

- "rerun": It is used to restart a failed or canceled workflow run.

- "cancel": It is used to cancel a currently running workflow.

In summary, the "gh run" command is a versatile tool that provides developers with complete control over workflow runs within their GitHub repositories. It enables them to manage and monitor the various automated workflows running in their repositories effectively. 

## tldr 
 
> View, run and watch recent GitHub Actions workflow runs.
> More information: <https://cli.github.com/manual/gh_run>.

- Interactively select a run to see information about the jobs:

`gh run view`

- Display information about a specific run:

`gh run view {{workflow_run_number}}`

- Display information about the steps of a job:

`gh run view --job={{job_number}}`

- Display the log of a job:

`gh run view --job={{job_number}} --log`

- Check a specific workflow and exit with a non-zero status if the run failed:

`gh run view {{workflow_run_number}} --exit-status && {{echo "run pending or passed"}}`

- Interactively select an active run and wait until it's done:

`gh run watch`

- Display the jobs for a run and wait until it's done:

`gh run watch {{workflow_run_number}}`

- Re-run a specific workflow:

`gh run rerun {{workflow_run_number}}`
