# stolonctl 
## chatgpt 
Stolonctl is a command-line tool used for managing the Stolon high availability postgresql cluster. 

The stolonctl command can be used to perform the following actions:

1. Initialize: This initializes a stolon cluster by creating a cluster definition file and initializing the first keeper instance.

2. Setup: This sets up a new standby keeper instance.

3. Add data: This adds data to the stolon cluster by adding a new PostgreSQL replica.

4. Start: This starts a keeper instance.

5. Stop: This stops a keeper instance.

6. Restart: This restarts a keeper instance.

7. Promote: This promotes a PostgreSQL replica to be the new primary in the cluster.

8. Remove data: This removes a postgres replica from the stolon cluster.

9. Status: This displays the status of the stolon cluster.

10. Edit: This edits the cluster definition file.

11. Validate: This validates the cluster status.

12. Backup: This creates a backup of the primary PostgreSQL instance.

To use stolonctl, you need to have a stolon cluster already set up and running. You also need to have stolonctl installed on the machine where you want to execute the command. The stolonctl command is usually used by a cluster administrator or a developer who is responsible for maintaining the stolon cluster. 

## tldr 
 
> CLI for Stolon, a cloud native PostgreSQL manager for PostgreSQL high availability.
> More information: <https://github.com/sorintlab/stolon>.

- Get cluster status:

`stolonctl --cluster-name {{cluster_name}} --store-backend {{store_backend}} --store-endpoints {{store_endpoints}} status`

- Get cluster data:

`stolonctl --cluster-name {{cluster_name}} --store-backend {{store_backend}} --store-endpoints {{store_endpoints}} clusterdata`

- Get cluster specification:

`stolonctl --cluster-name {{cluster_name}} --store-backend {{store_backend}} --store-endpoints {{store_endpoints}} spec`

- Update cluster specification with a patch in JSON format:

`stolonctl --cluster-name {{cluster_name}} --store-backend {{store_backend}} --store-endpoints {{store_endpoints}} update --patch '{{cluster_spec}}'`
