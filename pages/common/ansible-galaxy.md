# ansible-galaxy 
## chatgpt 
The `ansible-galaxy` command is a tool that comes with Ansible that is used for managing external roles. Roles are a reusable and sharable unit of Ansible content that can be used to organize and run Ansible tasks. Ansible Galaxy is a platform where Ansible roles created by the community can be shared and downloaded from.

The `ansible-galaxy` command has several sub-commands, including:

- `init`: Creates a new role directory structure. This includes the necessary directories and files required for the role to work.

- `install`: Installs one or multiple roles from Galaxy, either by specifying the role names or by reading them from a `requirements.yml` file.

- `remove`: Removes one or multiple roles from the system.

- `search`: Searches for roles available on Ansible Galaxy, based on specific keywords.

- `info`: Displays information about a specific role, such as the role's name, author, description, and version.

- `list`: Lists all roles installed on the system.

- `import`: Imports an external role into the current project.

Using `ansible-galaxy`, users can easily download new roles from the Ansible Galaxy community and integrate them into their projects. The command also simplifies the installation, configuration, and management of roles by automating many of the needed steps, such as creating the required folder structure and installing any necessary dependencies. 

## tldr 
 
> Create and manage Ansible roles.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

- Install a role:

`ansible-galaxy install {{username}}.{{role_name}}`

- Remove a role:

`ansible-galaxy remove {{username}}.{{role_name}}`

- List installed roles:

`ansible-galaxy list`

- Search for a given role:

`ansible-galaxy search {{role_name}}`

- Create a new role:

`ansible-galaxy init {{role_name}}`

- Get information about a user role:

`ansible-galaxy role info {{username}}.{{role_name}}`

- Get information about a collection:

`ansible-galaxy collection info {{username}}.{{collection_name}}`
