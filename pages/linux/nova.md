# nova 
## chatgpt 
The "nova" command is a command-line tool used to manage OpenStack Compute resources, such as instances, images, and flavors. 

Here are some common subcommands and options used with the "nova" command:

- "nova list": displays a list of all instances in the OpenStack Compute environment
- "nova boot": creates a new instance, specifying parameters like flavor, image, and network configuration
- "nova image-create": creates a new image from an existing instance
- "nova flavor-create": creates a new flavor that can be used when launching instances
- "nova show": displays detailed information about a specific instance
- "-h" or "--help": provides help and usage information for the nova command and its subcommands

Overall, the "nova" command is a powerful tool for managing and configuring resources in an OpenStack Compute environment. 

## tldr 
 
> The OpenStack project that provides a way to provision compute instances.
> More information: <https://docs.openstack.org/nova/latest/>.

- List VMs on current tenant:

`nova list`

- List VMs of all tenants (admin user only):

`nova list --all-tenants`

- Boot a VM on a specific host:

`nova boot --nic net-id={{net_id}} --image {{image_id}} --flavor {{flavor}} --availability-zone nova:{{host_name}} {{vm_name}}`

- Start a server:

`nova start {{server}}`

- Stop a server:

`nova stop {{server}}`

- Attach a network interface to a specific VM:

`nova interface-attach --net-id {{net_id}} {{server}}`
