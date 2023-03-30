# cgcreate 
## chatgpt 
The "cgcreate" command is used in Linux systems to create a new cgroup (control group). 

Cgroups are a Linux kernel feature that allows users to limit, allocate, and prioritize system resources such as CPU, memory, and disk I/O among a group of processes. By creating cgroups, you can define limits on these resources, and allocate them to specific tasks, users or applications. 

To use the "cgcreate" command, you need to have the "cgroup-tools" package installed. Once installed, you can create a new cgroup by running the following command:

cgcreate -g [subsystem:][name]

Where: 
- [subsystem]: denotes the cgroup subsystem you want to use. Examples of subsystems include cpu, memory, devices, cpuset, etc. If you don't specify a subsystem, the cgroup is created in all subsystems.
- [name]: is the name you want to give to your new cgroup. 

Here's an example of how to create a cgroup for CPU usage:

sudo cgcreate -g cpu:/my_cgroup

This creates a new cgroup called "my_cgroup" in the CPU subsystem. You can now set the CPU usage limits for this cgroup using the "cgset" command.

Note that you need to have root or sudo privileges to create cgroups. 

## tldr 
 
> Create cgroups, used to limit, measure, and control resources used by processes.
> `cgroups` types can be `memory`, `cpu`, `net_cls`, etc.
> More information: <https://manned.org/cgcreate>.

- Create a new group:

`cgcreate -g {{group_type}}:{{group_name}}`

- Create a new group with multiple cgroup types:

`cgcreate -g {{group_type1}},{{group_type2}}:{{group_name}}`

- Create a subgroup:

`mkdir /sys/fs/cgroup/{{group_type}}/{{group_name}}/{{subgroup_name}}`
