# aws s3 
## chatgpt 
The AWS S3 command-line interface (CLI) is a tool that enables the management of S3 buckets and objects from the command line. The command "aws s3" is the basic syntax for using the AWS S3 CLI.

When using the "aws s3" command, several subcommands can be used to perform different operations, such as:

1. Copying objects between S3 buckets or folders within a bucket.
2. Uploading or downloading files from S3 buckets.
3. Deleting objects or entire buckets.
4. Configuring bucket permissions and access control.
5. Listing and retrieving object metadata.

To use the "aws s3" command, you must first have an active AWS account with access to the S3 service. You must also have the AWS CLI installed on your local machine, which can be installed using a package manager or downloaded from the AWS documentation.

Once installed, the "aws s3" command and its subcommands can be used to manage S3 buckets and objects using a shell or terminal interface. For example, the command "aws s3 ls" can be used to list all S3 buckets in an account, while "aws s3 cp <local-path> <s3-path>" can be used to copy a local file to an S3 bucket. 

## tldr 
 
> CLI for AWS S3 - provides storage through web services interfaces.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3/index.html>.

- Show files in a bucket:

`aws s3 ls {{bucket_name}}`

- Sync files and directories from local to bucket:

`aws s3 sync {{path/to/files}} s3://{{bucket_name}}`

- Sync files and directories from bucket to local:

`aws s3 sync s3://{{bucket_name}} {{path/to/target}}`

- Sync files and directories with exclusions:

`aws s3 sync {{path/to/files}} s3://{{bucket_name}} --exclude {{path/to/file}} --exclude {{path/to/directory}}/*`

- Remove file from bucket:

`aws s3 rm s3://{{bucket}}/{{path/to/file}}`

- Preview changes only:

`aws s3 {{any_command}} --dryrun`
