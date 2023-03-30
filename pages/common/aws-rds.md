# aws rds 
## chatgpt 
The "aws rds" command is used to interact with Amazon Web Services (AWS) Relational Database Service (RDS). RDS is a fully managed relational database service that is compatible with various databases like MySQL, PostgreSQL, MariaDB, Oracle, and more.

When you use the "aws rds" command, you can do the following:

1. Create a new RDS instance.
2. Modify an existing RDS instance.
3. Delete an RDS instance.
4. List all available RDS instances.
5. Create a new RDS database.
6. Modify an existing database.
7. Delete a database.
8. Take a snapshot of an RDS instance or database.
9. Restore from an RDS snapshot.
10. Manage RDS DB instances, DB snapshots, DB parameter groups, and DB events.

Overall, the "aws rds" command is a powerful tool for managing your databases in the cloud with ease and efficiency. 

## tldr 
 
> CLI for AWS Relational Database Service.
> Create and manage relational databases.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/rds/index.html>.

- Show help for specific RDS subcommand:

`aws rds {{subcommand}} help`

- Stop instance:

`aws rds stop-db-instance --db-instance-identifier {{instance_identifier}}`

- Start instance:

`aws rds start-db-instance --db-instance-identifier {{instance_identifier}}`

- Modify an RDS instance:

`aws rds modify-db-instance --db-instance-identifier {{instance_identifier}} {{parameters}} --apply-immediately`

- Apply updates to an RDS instance:

`aws rds apply-pending-maintenance-action --resource-identifier {{database_arn}} --apply-action {{system-update}} --opt-in-type {{immediate}}`

- Change an instance identifier:

`aws rds modify-db-instance --db-instance-identifier {{old_instance_identifier}} --new-db-instance-identifier {{new_instance_identifier}}`

- Reboot an instance:

`aws rds reboot-db-instance --db-instance-identifier {{instance_identifier}}`

- Delete an instance:

`aws rds delete-db-instance --db-instance-identifier {{instance_identifier}} --final-db-snapshot-identifier {{snapshot_identifier}} --delete-automated-backups`
