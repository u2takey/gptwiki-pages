# terraform 
## chatgpt 
Terraform is an open-source infrastructure as code software tool that provides a consistent CLI to manage various popular services and software stacks. It enables users to define infrastructure as code (IaC) and create, change, and improve infrastructure across multiple providers using a single configuration file.

When you run the command "terraform", it will look for a configuration file called main.tf in the current directory. This file contains a set of instructions that describe the desired infrastructure state. Terraform then reads this file and creates a plan to create, modify, or delete infrastructure resources based on the defined state.

The configuration file typically includes the following:

1. Provider blocks: These blocks define which infrastructure providers Terraform will use to create the resources. Providers could be AWS, Google Cloud Platform, Microsoft Azure etc.
2. Resource blocks: These blocks define the infrastructure resources that Terraform will create, modify, or delete. Examples of resources include EC2 instances, S3 buckets, and VPCs.
3. Variables: These blocks allow you to define variables, which can be used in the configuration file and passed as arguments to Terraform commands.
4. Outputs: These blocks allow you to define output values that are returned by Terraform after the infrastructure is created.

Once you have created your configuration file, you can run Terraform commands to create or modify infrastructure resources. Some of the most commonly used commands include:

- terraform init: Initializes the working directory with necessary configuration files and downloads the required providers.
- terraform plan: Creates a plan to create, modify, or delete infrastructure resources based on the defined state in the configuration file.
- terraform apply: Applies the changes defined in the plan to create, modify, or delete infrastructure resources.
- terraform destroy: Destroys the infrastructure resources created by Terraform.

In summary, the terraform command is used to interact with the Terraform CLI, which allows you to define and manage infrastructure resources in a consistent and reproducible manner. It can be customized using a configuration file and provides a wide range of commands for creating, modifying, and destroying infrastructure. 

## tldr 
 
> Create and deploy infrastructure as code to cloud providers.
> More information: <https://www.terraform.io/>.

- Initialize a new or existing Terraform configuration:

`terraform init`

- Verify that the configuration files are syntactically valid:

`terraform validate`

- Format configuration according to Terraform language style conventions:

`terraform fmt`

- Generate and show an execution plan:

`terraform plan`

- Build or change infrastructure:

`terraform apply`

- Destroy Terraform-managed infrastructure:

`terraform destroy`
