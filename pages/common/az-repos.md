# az repos 
## chatgpt 
"az repos" is a command in the Azure Command-Line Interface (CLI) tool that is used to manage code repositories in Azure DevOps. It offers a set of commands that enable users to manage repositories, files, and other related features.

Some of the common commands available in "az repos" include:

1. create: This command permits users to create a new Git repository in Azure DevOps.

2. import: This command is used to import existing Git repositories from other sources into Azure DevOps.

3. list: This command is used to list all repositories available in Azure DevOps.

4. delete: This command is used to delete a repository.

5. clone: This command enables the user to clone a repository from Azure DevOps to their local machine.

6. show: This command displays the details of a particular repository.

7. set-policy: This command is used to set repository policies for a particular repository, including branch restrictions, code quality rules, and security policies.

Overall, "az repos" offers a set of powerful commands that allow developers to manage their code repositories easily, quickly, and efficiently. 

## tldr 
 
> Manage Azure DevOps repos.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/en-us/cli/azure/repos?view=azure-cli-latest>.

- List all repos in a specific project:

`az repos list --project {{project_name}}`

- Add policy on a specific branch of a specific repository to restrict basic merge:

`az repos policy merge-strategy create --repository-id {{repository_id_in_repos_list}} --branch {{branch_name}} --blocking --enabled --allow-no-fast-forward false --allow-rebase true --allow-rebase-merge true --allow-squash true`

- Add build validation on a specific repository, using an existing build pipeline, to be triggered automatically on source update:

`az repos policy build create --repository-id {{repository_id}} --build-definition-id {{build_pipeline_id}} --branch main --blocking --enabled --queue-on-source-update-only true --display-name {{name}} --valid-duration {{minutes}}`

- List all active Pull Requests on a specific repository within a specific project:

`az repos pr list --project {{project_name}} --repository {{repository_name}} --status active`
