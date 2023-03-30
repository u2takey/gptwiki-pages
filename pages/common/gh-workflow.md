# gh workflow 
## chatgpt 
The gh workflow command is a command that is available in the GitHub CLI (Command Line Interface). This command allows you to create, view, and manage the GitHub Actions workflows for a specific repository.

The syntax for this command is as follows:

```
gh workflow [flags]
```

The available flags for this command are:

- `status`: Displays the status of the most recent workflow run.
- `view`: Displays the details of a specific workflow run.
- `list`: Lists all of the available workflows for the current repository.
- `disable`: Disables a specific workflow.
- `enable`: Enables a specific workflow.

To use this command, you must have the GitHub CLI installed and authenticated with your GitHub account. Once authenticated, you can navigate to the repository you want to manage the workflows for and execute the command with the appropriate flag.

For example, to view the most recent workflow run for a repository, you would use the following command:

```
gh workflow status
```

This will display the status of the most recent workflow run, including whether it succeeded or failed, when it was run, and any relevant logs or output.

Similarly, to list all available workflows for the repository, you would use the following command:

```
gh workflow list
```

This will display a list of all the workflows available for the repository, along with information about when they were last run and their current status.

Overall, the `gh workflow` command is a powerful tool for managing GitHub Actions workflows from the command line, allowing you to quickly view status, disable or enable workflows, and more. 

## tldr 
 
> List, view, and run GitHub Actions workflows.
> More information: <https://cli.github.com/manual/gh_workflow>.

- Interactively select a workflow to view the latest jobs for:

`gh workflow view`

- View a specific workflow in the default browser:

`gh workflow view {{id|workflow_name|filename.yml}} --web`

- Display the YAML definition of a specific workflow:

`gh workflow view {{id|workflow_name|filename.yml}} --yaml`

- Display the YAML definition for a specific Git branch or tag:

`gh workflow view {{id|workflow_name|filename.yml}} --ref {{branch|tag_name}} --yaml`

- List workflow files (use `--all` to include disabled workflows):

`gh workflow list`

- Run a manual workflow with parameters:

`gh workflow run {{id|workflow_name|filename.yml}} {{--raw-field param1=value1 --raw-field param2=value2 ...}}`

- Run a manual workflow using a specific branch or tag with JSON parameters from `stdin`:

`echo '{{{"param1": "value1", "param2": "value2", ...}}}' | gh workflow run {{id|workflow_name|filename.yml}} --ref {{branch|tag_name}}`

- Enable or disable a specific workflow:

`gh workflow {{enable|disable}} {{id|workflow_name|filename.yml}}`
