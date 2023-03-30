# cloud-init 
## chatgpt 
cloud-init is an open-source package that is used for providing initialization metadata to cloud instances. It is a tool that helps in launching and configuring cloud instances in a platform-independent way. The primary function of cloud-init is to start the cloud instance and configure it on first boot. It works with various cloud providers, including Amazon Web Services (AWS), Google Cloud Platform (GCP), and OpenStack.

The cloud-init command is used to configure cloud instances on first boot. It reads the metadata from the cloud provider and performs the necessary operations to configure the instance, such as setting the hostname, creating users, installing packages, and configuring network settings. The metadata can be in various formats such as a cloud-config file or a user-data script.

Here is an example of using the cloud-init command in AWS to launch a new EC2 instance:

```
aws ec2 run-instances --image-id ami-0a91cd140a1fc148a \
--instance-type t2.micro \
--key-name my-key-pair \
--security-group-ids sg-0b34d27c4a4d9367a \
--subnet-id subnet-010d1f762856e055c \
--user-data file://cloud-config.yml
```

In this example, the `user-data` parameter specifies the cloud-config file `cloud-config.yml` that contains instructions for configuring the instance. When the instance is launched, cloud-init reads this file and performs the specified operations to configure the instance.

Overall, cloud-init is a powerful tool that enables platform-independent configuration of cloud instances and makes it easier to launch and manage cloud infrastructure. 

## tldr 
 
> Command line tool for managing cloud instance initialization.
> More information: <https://cloudinit.readthedocs.io>.

- Display the status of the most recent cloud-init run:

`cloud-init status`

- Wait for cloud-init to finish running and then report status:

`cloud-init status --wait`

- List available top-level metadata keys to query:

`cloud-init query --list-keys`

- Query cached instance metadata for data:

`cloud-init query {{dot_delimited_variable_path}}`

- Clean logs and artifacts to allow cloud-init to rerun:

`cloud-init clean`
