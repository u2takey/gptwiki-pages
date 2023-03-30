# doctl compute droplet 
## chatgpt 
The `doctl compute droplet` command is used to manage DigitalOcean droplets from the command line using the DigitalOcean API. 

- `doctl`: This is the official DigitalOcean command-line tool.
- `compute`: It is one of the categories of commands available in `doctl`. It allows managing DigitalOcean resources related to computing, like droplets, load balancers, and firewalls.
- `droplet`: A droplet is DigitalOcean's terminology for virtual servers (VMs), which can be created, deleted, and managed using `doctl compute droplet`.

The `doctl compute droplet` command can be used with various sub-commands like `create`, `list`, `delete`. Here are some common sub-commands:

- `create`: It is used to create a new droplet based on an image, size, region, and other optional parameters specified on the command-line. For example, `doctl compute droplet create my-droplet --image ubuntu-20-04-x64 --size s-1vcpu-1gb --region nyc1`
- `list`: It is used to list all the available droplets in a DigitalOcean account. For example, `doctl compute droplet list`
- `delete`: It is used to delete a droplet by its ID or name. For example, `doctl compute droplet delete my-droplet`


There are many other options available with `doctl compute droplet` command, which can be accessed by running `doctl compute droplet` without any sub-commands or by checking the official documentation. 

## tldr 
 
> List, create, and delete virtual machines which are called droplets.
> More information: <https://docs.digitalocean.com/reference/doctl/reference/compute/droplet/>.

- Create a droplet:

`doctl compute droplet create --region {{region}} --image {{os_image}} --size {{vps_type}} {{droplet_name}}`

- Delete a droplet:

`doctl compute droplet delete {{droplet_id|droplet_name}}`

- List droplets:

`doctl compute droplet list`
