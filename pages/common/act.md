# act 
## chatgpt 
As an AI language model, I presume you are asking about the "act" command in a specific context. There are several meanings and contexts for the term "act", so please provide more details about the specific context or use case, and I will provide a detailed explanation of the command. 

## tldr 
 
> Execute GitHub Actions locally using Docker.
> More information: <https://github.com/nektos/act>.

- List the available actions:

`act -l`

- Run the default event:

`act`

- Run a specific event:

`act {{event_type}}`

- Run a specific action:

`act -a {{action_id}}`

- Do not actually run the actions (i.e. a dry run):

`act -n`

- Show verbose logs:

`act -v`

- Run a specific workflow:

`act push -W {{path/to/workflow}}`
