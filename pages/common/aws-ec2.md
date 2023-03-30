# aws ec2 
## chatgpt 
"aws ec2" is a command-line interface (CLI) command used to interact with Amazon Web Services Elastic Compute Cloud (EC2) to manage cloud-based virtual servers. It provides a range of options for configuring, launching, and managing EC2 instances.

Some examples of the types of actions you can perform with "aws ec2" include:

- Launching and terminating EC2 instances
- Configuring and attaching storage volumes to EC2 instances
- Managing EC2 instance security settings using security groups
- Managing Elastic IP addresses and assigning them to EC2 instances
- Using the AWS CLI to monitor the status and health of your EC2 instances.

To use the "aws ec2" command, you will need to have the AWS CLI installed on your computer, as well as the necessary credentials (Access Key and Secret Access Key) to authenticate with AWS. You can then use the "aws ec2" command followed by options and arguments to specify the specific EC2 instance or resource you want to manage. 

## tldr 
 
> CLI for AWS EC2.
> Provides secure and resizable computing capacity in the AWS cloud to enable faster development and deployment of applications.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ec2/index.html>.

- Display information about a specific instance:

`aws ec2 describe-instances --instance-ids {{instance_id}}`

- Display information about all instances:

`aws ec2 describe-instances`

- Display information about all EC2 volumes:

`aws ec2 describe-volumes`

- Delete an EC2 volume:

`aws ec2 delete-volume --volume-id {{volume_id}}`

- Create a snapshot from an EC2 volume:

`aws ec2 create-snapshot --volume-id {{volume_id}}`

- List available AMIs (Amazon Machine Images):

`aws ec2 describe-images`

- Show list of all available EC2 commands:

`aws ec2 help`

- Show help for specific EC2 subcommand:

`aws ec2 {{subcommand}} help`
