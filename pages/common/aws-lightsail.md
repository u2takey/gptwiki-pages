# aws lightsail 
## chatgpt 
AWS Lightsail is a service that provides an easy and affordable way to create, launch and manage virtual private servers (VPS) with Amazon Web Services. The command "aws lightsail" is used to access the AWS Lightsail API from the command line interface (CLI). 

When you enter "aws lightsail" on the command line, you will be prompted to enter any additional commands you wish to execute, such as "create-instance" or "delete-instance". These commands will perform specific actions within the Lightsail service using the API, such as creating or deleting a VPS instance. 

You can also use the "aws lightsail" command to access and manage other features of the service, such as networking, storage, and load balancers. Overall, the "aws lightsail" command is a critical tool for managing your VPSs and related resources within the AWS cloud ecosystem. 

## tldr 
 
> Manage Amazon Lightsail resources using the CLI.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/lightsail/index.html>.

- List all virtual private servers, or instances:

`aws lightsail get-instances`

- List all bundles (instance plans):

`aws lightsail list-bundles`

- List all available instance images, or blueprints:

`aws lightsail list-blueprints`

- Create an instance:

`aws lightsail create-instances --instance-names {{name}} --availability-zone {{region}} --bundle-id {{nano_2_0}} --blueprint-id {{blueprint_id}}`

- Print the state of a specific instance:

`aws lightsail get-instance-state --instance-name {{name}}`

- Stop a specific instance:

`aws lightsail stop-instance --instance-name {{name}}`

- Delete a specific instance:

`aws lightsail delete-instance --instance-name {{name}}`
