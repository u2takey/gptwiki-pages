# sacctmgr 
## chatgpt 
sacctmgr is a command-line utility that is used to manage and administer the Slurm Accounting Manager daemon (sacctmd). sacctmgr provides a set of administrative commands that allow users to:

- Add, modify and remove user accounts, associations, and clusters.
- Define and manage user charges.
- Monitor and control the daemons and services associated with the Slurm accounting system.

Here are some of the most commonly used sacctmgr commands:

- add - Add users, accounts, clusters, and associations to the Slurm accounting system.
- modify - Modify user accounts, associations, and clusters.
- show - Display information about users, accounts, clusters, and associations.
- delete - Remove users, accounts, or associations from the Slurm accounting system.
- set - Set attributes for users, accounts, and associations.
- ping - Check the connectivity between the sacctmgr server and the Slurm database.
- list - List users, accounts, and associations.

Overall, sacctmgr is a powerful administrative tool for managing the Slurm accounting system, and it is essential to have a good understanding of its commands and options to effectively manage Slurm clusters. 

## tldr 
 
> View, setup, and manage Slurm accounts.
> More information: <https://slurm.schedmd.com/sacctmgr.html>.

- Show current configuration:

`sacctmgr show configuration`

- Add a cluster to the slurm database:

`sacctmgr add cluster {{cluster_name}}`

- Add an account to the slurm database:

`sacctmgr add account {{account_name}} cluster={{cluster_of_account}}`

- Show details of user/association/cluster/account using a specific format:

`sacctmgr show {{user|association|cluster|account}} format="Account%10" format="GrpTRES%30"`
