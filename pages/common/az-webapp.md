# az webapp 
## chatgpt 
az webapp is a command used in the Azure CLI (Command Line Interface) tool to perform operations on Azure Web Apps. Web Apps in Azure are a service that allows developers to build, deploy, and run web applications on the cloud. The az webapp command provides a set of subcommands to perform various tasks such as creating a new Web App, deploying or updating an existing Web App, managing Web App configurations, scaling the Web App, or monitoring its performance.

Some of the commonly used subcommands with the az webapp command are:

- create: This subcommand is used to create a new Web App in Azure. It requires parameters such as name, resource group, runtime stack, and other configurations.
- deploy: This subcommand is used to deploy a code or container image to an existing Web App. It can deploy code from a local repository, Azure DevOps, GitHub, or other sources.
- config: This subcommand is used to configure various settings of an existing Web App such as connection strings, environment variables, custom domains, SSL certificates, and more.
- scale: This subcommand is used to scale the Web App horizontally or vertically based on the traffic and workload. It can scale up or down the number of instances, CPU cores, and memory size.
- show: This subcommand is used to display the details of an existing Web App such as name, resource group, runtime stack, URL, status, and other properties.

Overall, the az webapp command is a powerful tool for managing Azure Web Apps from the command line, which allows developers and DevOps professionals to automate the deployment, configuration, scaling, and monitoring of their applications on the cloud. 

## tldr 
 
> Manage Web Applications hosted in Azure Cloud Services.
> Part of `azure-cli`.
> Mode information: <https://learn.microsoft.com/cli/azure/webapp>.

- List available runtimes for a web application:

`az webapp list-runtimes --os-type {{windows|linux}}`

- Create a web application:

`az webapp up --name {{name}} --location {{location}} --runtime {{runtime}}`

- List all web applications:

`az webapp list`

- Delete a specific web application:

`az webapp delete --name {{name}} --resource-group {{resource_group}}`
