# pyinfra 
## chatgpt 
`pyinfra` is a tool used for automating infrastructure deployment and configuration. It uses Python to describe and execute these tasks, making it easy to write reusable, dynamic infrastructure-as-code scripts and modules.

To use `pyinfra`, you start by writing a Python script that describes the infrastructure you want to manage. This script can use any Python library or module to perform tasks, including running shell commands, managing files, and interacting with APIs.

Once you have written your script, you can run `pyinfra` to execute it on your infrastructure. `pyinfra` uses a modular architecture based on plugins, allowing you to extend it with additional functionality as needed.

Some common use cases for `pyinfra` include:

- Provisioning and configuring servers and services
- Managing containers and virtual machines
- Automating backups and disaster recovery
- Deploying updates and patches to infrastructure
- Monitoring and reporting on infrastructure status and performance

Overall, `pyinfra` is a powerful tool for managing infrastructure in a dynamic, flexible, and efficient way. 

## tldr 
 
> Automates infrastructure at a large scale.
> More information: <https://docs.pyinfra.com>.

- Execute a command over SSH:

`pyinfra {{target_ip_address}} exec -- {{command_name_and_arguments}}`

- Execute contents of a deploy file on a list of targets:

`pyinfra {{path/to/target_list.py}} {{path/to/deploy.py}}`

- Execute commands on locally:

`pyinfra @local {{path/to/deploy.py}}`

- Execute commands over Docker:

`pyinfra @docker/{{container}} {{path/to/deploy.py}}`
