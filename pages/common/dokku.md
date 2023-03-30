# dokku 
## chatgpt 
As an AI language model, I cannot execute commands or access a terminal as it requires a system interaction. However, I can break down what the command "dokku" means.

Dokku is a command-line tool used for deploying and managing applications on a single server. It's an open-source Container Platform as a Service (PaaS) that provides developers with a simple and effective way to deploy and manage apps on their own infrastructure. Dokku relies on Heroku Buildpacks and Docker to deploy apps on a single server.

The dokku command allows users to interact with the Dokku platform to manage their applications, deploy code, create and manage databases, configure environment variables, and much more.

Overall, dokku simplifies the deployment and management of web applications on a single server, making it a popular choice for developers who don't want to use a more complicated PaaS solution. 

## tldr 
 
> Docker powered mini-Heroku (PaaS).
> Easily deploy multiple apps to your server in different languages using a single `git-push` command.
> More information: <https://github.com/dokku/dokku>.

- List running apps:

`dokku apps`

- Create an app:

`dokku apps:create {{app_name}}`

- Remove an app:

`dokku apps:destroy {{app_name}}`

- Install plugin:

`dokku plugin:install {{full_repo_url}}`

- Link database to an app:

`dokku {{db}}:link {{db_name}} {{app_name}}`
