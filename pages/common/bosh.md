# bosh 
## chatgpt 
BOSH is a command-line tool used to deploy and manage cloud software. It is used particularly for deployment and management of large distributed systems.

When you run the command "bosh", it will open the BOSH CLI (Command Line Interface) shell, which provides various commands to manage the cloud infrastructure. These commands include:

1. bosh target: This command is used to set the target BOSH director that you want to connect to.

2. bosh deploy: This command is used to deploy a release on your infrastructure.

3. bosh delete-deployment: This command is used to delete an existing deployment.

4. bosh run-errand: This command is used to run a specific errand in a deployment.

5. bosh ssh: This command is used to SSH into a VM in the deployment.

6. bosh logs: This command is used to retrieve logs from a deployment.

These are just some of the many commands available through BOSH. BOSH is particularly useful because it abstracts away the underlying infrastructure layer, allowing developers to focus on the application layer. 

## tldr 
 
> Command-line tool to deploy and manage the bosh director.
> More information: <https://bosh.io/docs/cli-v2/>.

- Create local alias for director:

`bosh alias-env {{environment_name}} -e {{ip_address|url}} --ca-cert {{ca_certificate}}`

- List environments:

`bosh environments`

- Log in to the director:

`bosh login -e {{environment}} `

- List deployments:

`bosh -e {{environment}} deployments`

- List environment virtual machines:

`bosh -e {{environment}} vms -d {{deployment}}`

- Ssh into virtual machine:

`bosh -e {{environment}} ssh {{virtual_machine}} -d {{deployment}}`

- Upload stemcell:

`bosh -e {{environment}} upload-stemcell {{stemcell_file|url}}`

- Show current cloud config:

`bosh -e {{environment}} cloud-config`
