# az pipelines 
## chatgpt 
The command "az pipelines" is a sub-command provided by Azure DevOps CLI that allows managing Azure pipelines, which are essentially automated workflows that provide a streamlined way of building, testing, and deploying applications. 

This command provides a set of options and sub-commands to manage various aspects of pipelines, such as creating and deleting pipelines, configuring pipeline settings, and managing pipeline artifacts.

Some of the commonly used sub-commands and options of "az pipelines" command include:

- "create": This sub-command allows creating a new pipeline definition.
- "delete": This sub-command allows deleting an existing pipeline definition.
- "configure": This sub-command allows configuring pipeline settings, such as agents, triggers, and permissions.
- "run": This sub-command allows queuing a new build or release pipeline run.
- "show": This sub-command allows displaying the details of a pipeline definition.

Overall, the "az pipelines" command allows automating and managing the pipeline lifecycle effectively using the Azure DevOps CLI. 

## tldr 
 
> Manage Azure Pipelines resources.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/pipelines>.

- Create a new Azure Pipeline (YAML based):

`az pipelines create --org {{organization_url}} --project {{project_name}} --name {{pipeline_name}} --description {{description}} --repository {{repository_name}} --branch {{branch_name}}`

- Delete a specific pipeline:

`az pipelines delete --org {{organization_url}} --project {{project_name}} --id {{pipeline_id}}`

- List pipelines:

`az pipelines list --org {{organization_url}} --project {{project_name}}`

- Enqueue a specific pipeline to run:

`az pipelines run --org {{organization_url}} --project {{project_name}} --name {{pipeline_name}}`

- Get the details of a specific pipeline:

`az pipelines show --org {{organization_url}} --project {{project_name}} --name {{pipeline_name}}`

- Update a specific pipeline:

`az pipelines update --org {{organization_url}} --project {{project_name}} --name {{pipeline_name}} --new-name {{pipeline_new_name}} --new-folder-path {{user1/production_pipelines}}`

- Get a list of agents in a pool:

`az pipelines agent list --org {{organization_url}} --pool-id {{agent_pool}}`
