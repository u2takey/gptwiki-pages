# gh auth 
## chatgpt 
The `gh auth` command is a command-line tool provided by GitHub that allows users to authenticate with a GitHub account via a token or a web authentication flow. 

This command provides a way for users to input and store their GitHub authentication credentials securely on their local machine, which can then be used to interact with the GitHub API and access resources that are otherwise protected.

When you run the `gh auth` command, it will launch an interactive setup process that guides you through the process of authenticating with GitHub. The setup process will prompt you to choose an authentication method, such as a personal access token or web authentication, and then guides you through the process of providing the necessary credentials.

Once the setup process is complete, you can use the credentials stored on your machine to perform various actions on GitHub, such as cloning repositories, pushing changes, creating issues, managing pull requests, etc.

In summary, `gh auth` is a powerful command-line tool that empowers users to securely authenticate with GitHub, and access resources and perform tasks without hassle. 

## tldr 
 
> Authenticate with a GitHub host from the command-line.
> More information: <https://cli.github.com/manual/gh_auth>.

- Log in with interactive prompt:

`gh auth login`

- Log in with a token from standard input (created in https://github.com/settings/tokens):

`echo {{your_token}} | gh auth login --with-token`

- Check if you are logged in:

`gh auth status`

- Log out:

`gh auth logout`

- Log in with a specific GitHub Enterprise Server:

`gh auth login --hostname {{github.example.com}}`

- Refresh the session to ensure authentication credentials have the correct minimum scopes (removes additional scopes requested previously):

`gh auth refresh`

- Expand the permission scopes:

`gh auth refresh --scopes {{repo,admin:repo_hook,admin:org,admin:public_key,admin:org_hook,...}}`
