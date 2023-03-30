# cf 
## chatgpt 
The command "cf" is a command-line interface used to interact with the Cloud Foundry platform. It is used to manage applications, services, and various aspects of the platform. Some common uses of "cf" are:

- "cf login": This command is used to log in to a Cloud Foundry instance. It prompts the user for their username and password and authenticates them with the platform. Once authenticated, the user can start using "cf" to interact with their applications and services.

- "cf push": This command is used to deploy an application to the Cloud Foundry platform. It packages the application and its dependencies into a buildpack, which is then deployed to the platform. Once deployed, the application can be started and stopped using "cf".

- "cf apps": This command is used to list all the applications deployed on the Cloud Foundry platform. It provides information such as the application name, the URL where the application can be accessed, the status of the application, and the amount of memory and CPU it is currently using.

- "cf services": This command is used to list all the services available on the Cloud Foundry platform. A service is a resource that an application can use, such as a database, a queue, or a cache.

- "cf marketplace": This command is used to list all the services available in the Cloud Foundry marketplace. The marketplace is a list of third-party services that can be used on the platform.

Overall, the "cf" command is an essential tool for anyone who uses the Cloud Foundry platform, whether they are developers deploying applications or operators managing the platform. 

## tldr 
 
> Command-line tool to manage apps and services on Cloud Foundry.
> More information: <https://docs.cloudfoundry.org>.

- Log in to the Cloud Foundry API:

`cf login -a {{api_url}}`

- Push an app using the default settings:

`cf push {{app_name}}`

- View the services available from your organization:

`cf marketplace`

- Create a service instance:

`cf create-service {{service}} {{plan}} {{service_name}}`

- Connect an application to a service:

`cf bind-service {{app_name}} {{service_name}}`

- Run a script whose code is included in the app, but runs independently:

`cf run-task {{app_name}} "{{script_command}}" --name {{task_name}}`

- Start an interactive SSH session with a VM hosting an app:

`cf ssh {{app_name}}`

- View a dump of recent app logs:

`cf logs {{app_name}} --recent`
