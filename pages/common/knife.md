# knife 
## chatgpt 
`knife` is a command-line tool used in the Chef ecosystem for configuring, managing and interacting with Chef servers, nodes and the various components in between.

The knife command is used to perform various operations such as:

1. Managing the Cookbooks: You can use knife to manage the cookbooks in your Chef repository, and perform operations like uploading new cookbooks or deleting existing ones.
2. Managing Chef nodes: You can use knife to manage the various nodes in your Chef infrastructure. This includes listing nodes, creating new nodes or updating the attributes of existing ones.
3. Managing Roles: You can use knife to define, manage and update roles in your Chef infrastructure. Roles are used to group together and assign specific attributes and cookbooks to nodes.
4. Managing Chef environment: You can use knife to create, modify or delete different Chef environments, which are used to set up different configurations and variables for different nodes.
5. Running recipes on nodes: Knife can be used to run recipes selectively on specific nodes.
6. Other management tasks: Knife can be used to perform various other tasks in a Chef infrastructure such as managing data bags, managing SSL certificates, managing users etc.

To use the knife command, you need to have access to a Chef server and ensure that the necessary authentication credentials are set up correctly. You can access the various options and sub-commands of the knife command by using "knife --help" or "knife SUB-COMMAND --help". 

## tldr 
 
> CLI for interacting with a Chef server from a local Chef repo.
> More information: <https://docs.chef.io/knife.html>.

- Bootstrap a new node:

`knife bootstrap {{fqdn_or_ip}}`

- List all registered nodes:

`knife node list`

- Show a node:

`knife node show {{node_name}}`

- Edit a node:

`knife node edit {{node_name}}`

- Edit a role:

`knife role edit {{role_name}}`

- View a data bag:

`knife data bag show {{data_bag_name}} {{data_bag_item}}`

- Upload a local cookbook to the Chef server:

`knife cookbook upload {{cookbook_name}}`
