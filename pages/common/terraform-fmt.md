# terraform fmt 
## chatgpt 
The "terraform fmt" command is a Terraform command that is used to format Terraform configuration files for consistent and readable code. 

When run, the command checks all .tf and .tf.json files located in the current directory and its subdirectories to ensure that all the files are complying with the configured formatting rules. 

If any files are found to be impropely formatted, the command will automatically reformat them to follow the configured formatting rules.

This command is helpful as it helps developers maintain a consistent coding style and also makes it easier to spot and fix errors in the Terraform configuration files. 

## tldr 
 
> Format configuration according to Terraform language style conventions.
> More information: <https://www.terraform.io/docs/commands/fmt.html>.

- Format the configuration in the current directory:

`terraform fmt`

- Format the configuration in the current directory and subdirectories:

`terraform fmt -recursive`

- Display diffs of formatting changes:

`terraform fmt -diff`

- Do not list files that were formatted to `stdout`:

`terraform fmt -list=false`
