# gh api 
## chatgpt 
The command "gh api" is a command-line tool available in the GitHub CLI tool designed to interact with the GitHub API. 

When you run this command, it allows you to access and perform various operations on GitHub repositories, issues, pull requests, releases, and much more directly from your terminal. This command streamlines the process of making API requests and lets you interact with the GitHub API using simple commands.

To use this command, you need to have the GitHub CLI tool installed on your system. Once installed, you can access it by running 'gh api' followed by the API endpoint you want to access. Depending on the usage you specify, you can use an HTTP method such as GET, POST, or PATCH to send a request to the API.

For example, you can use the following command to fetch details of a particular repository:

```
gh api repos/owner/repository
```

This command sends a GET request to the GitHub API to fetch the details of the repository with the name "repository" owned by "owner".

Overall, the "gh api" command is a powerful tool that allows you to interact with the GitHub API directly from your command-line interface, making it faster and more efficient to work with GitHub repositories and other resources. 

## tldr 
 
> Makes authenticated HTTP requests to the GitHub API and prints the response.
> More information: <https://cli.github.com/manual/gh_api>.

- Display the subcommand help:

`gh api --help`

- Display the releases for the current repository in JSON format:

`gh api repos/:owner/:repo/releases`

- Create a reaction for a specific issue:

`gh api --header {{Accept:application/vnd.github.squirrel-girl-preview+json}} --raw-field '{{content=+1}}' {{repos/:owner/:repo/issues/123/reactions}}`

- Display the result of a GraphQL query in JSON format:

`gh api graphql --field {{name=':repo'}} --raw-field '{{query}}'`

- Send a request using a custom HTTP method:

`gh api --method {{POST}} {{endpoint}}`

- Include the HTTP response headers in the output:

`gh api --include {{endpoint}}`

- Do not print the response body:

`gh api --silent {{endpoint}}`

- Send a request to a specific GitHub Enterprise Server:

`gh api --hostname {{github.example.com}} {{endpoint}}`
