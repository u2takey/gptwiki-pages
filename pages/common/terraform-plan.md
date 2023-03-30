# terraform plan 
## chatgpt 
The `terraform plan` command is used in the Terraform infrastructure-as-code (IAC) tool to create an execution plan for the changes that you have made to your infrastructure code defined in Terraform configuration files. 

When executed, the Terraform plan command reads the current state of the infrastructure and compares it to the desired state defined in the configuration files. It then generates an execution plan that describes the actions Terraform will take to bring the actual state of the infrastructure into sync with the desired state. 

The output of the Terraform plan command lists all the changes that Terraform will make in response to the changes you specified in your Terraform configuration files. This includes creating new resources, updating existing resources, and deleting resources. 

Before applying the changes to your infrastructure, it's a good practice to run the Terraform plan command first to preview the changes that will be made, verify that they match your intentions, and avoid any unexpected changes. 

In summary, `terraform plan` is used to:

1. Generate a plan for applying changes to infrastructure code.
2. List all changes that Terraform will make to bring the actual state of the infrastructure into sync with the desired state.
3. Preview changes before applying them to avoid any unexpected changes. 

## tldr 
 
> Generate and show Terraform execution plans.
> More information: <https://www.terraform.io/docs/cli/commands/plan.html>.

- Generate and show the execution plan in the currently directory:

`terraform plan`

- Show a plan to destroy all remote objects that currently exist:

`terraform plan -destroy`

- Show a plan to update the Terraform state and output values:

`terraform plan -refresh-only`

- Specify values for input variables:

`terraform plan -var '{{name1}}={{value1}}' -var '{{name2}}={{value2}}'`

- Focus Terraform's attention on only a subset of resources:

`terraform plan -target {{resource_type.resource_name[instance index]}}`

- Output a plan as JSON:

`terraform plan -json`

- Write a plan to a specific file:

`terraform plan -no-color > {{path/to/file}}`
