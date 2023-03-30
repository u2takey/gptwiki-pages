# gh secret 
## chatgpt 
The `gh secret` command is used to interact with the GitHub Actions secrets in a repository. It allows you to create, delete, list, and view the values of secrets used in your GitHub Actions workflows.

Here are a few examples of how to use the `gh secret` command:

- `gh secret create`: This command is used to create a new secret in your repository. It requires two arguments: the name of the secret and its value. For example: `gh secret create MY_SECRET "my super secret value"`. The secret will be encrypted and securely stored in your repository settings.

- `gh secret delete`: This command deletes an existing secret. It requires the name of the secret as an argument. For example: `gh secret delete MY_SECRET`.

- `gh secret list`: This command lists all the secrets in your repository. It doesn't require any arguments. For example: `gh secret list`.

- `gh secret view`: This command allows you to view the value of a secret. It requires the name of the secret as an argument. For example: `gh secret view MY_SECRET`.

Overall, the `gh secret` command is a useful tool for managing sensitive information in your GitHub Actions workflows. It helps keep your code secure by allowing you to store and access secrets in a safe and encrypted manner. 

## tldr 
 
> Manage GitHub secrets from the command-line.
> More information: <https://cli.github.com/manual/gh_secret>.

- List secret keys for the current repository:

`gh secret list`

- List secret keys for a specific organization:

`gh secret list --org {{organization}}`

- List secret keys for a specific repository:

`gh secret list --repo {{owner}}/{{repository}}`

- Set a secret for the current repository (user will be prompted for the value):

`gh secret set {{name}}`

- Set a secret from a file for the current repository:

`gh secret set {{name}} < {{path/to/file}}`

- Set an organization secret for specific repositories:

`gh secret set {{name}} --org {{organization}} --repos {{repository1,repository2}}`

- Remove a secret for the current repository:

`gh secret remove {{name}}`

- Remove a secret for a specific organization:

`gh secret remove {{name}} --org {{organization}}`
