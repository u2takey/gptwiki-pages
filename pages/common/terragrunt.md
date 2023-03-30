# terragrunt 
## chatgpt 
Terragrunt is a command-line tool used to manage Terraform deployments. Here are some of the commonly used commands and their descriptions:

1. `terragrunt init`: This command initializes Terragrunt and creates a .terragrunt directory in your Terraform project. This directory contains a configuration file that defines how Terragrunt should interact with Terraform.

2. `terragrunt apply`: This command applies the Terraform configuration defined in your project. It creates or modifies resources, as specified in your Terraform code.

3. `terragrunt destroy`: This command destroys the Terraform resources defined in your project. It removes all resources created by your Terraform code.

4. `terragrunt plan`: This command generates a plan of the Terraform changes that will be made when you apply the configuration. It shows you how many resources will be created, modified, or destroyed.

5. `terragrunt output`: This command displays the output variables defined in your Terraform code. These variables can be used to pass information between Terraform projects.

6. `terragrunt validate`: This command validates the syntax of your Terraform code. It checks for any errors or warnings in your code.

7. `terragrunt state`: This command shows the current state of your Terraform resources. It displays the current values of your resources, including any changes that have been made since the resources were created.

Overall, Terragrunt provides a convenient way to manage and deploy Terraform code in a structured and consistent manner. 

## tldr 
 
> Keep your Terraform CLI arguments DRY.
> More information: <https://terragrunt.gruntwork.io>.

- Generate and show an execution plan:

`terragrunt plan`

- Build or change infrastructure:

`terragrunt apply`

- Show current deployment (from state):

`terragrunt show`

- Show module output values:

`terragrunt output`

- Destroy Terraform-managed infrastructure:

`terragrunt destroy`

- Build or change infrastructure from a tree of Terragrunt modules (stack):

`terragrunt run-all apply`
