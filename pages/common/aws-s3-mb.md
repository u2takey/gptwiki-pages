# aws s3 mb 
## chatgpt 
The "aws s3 mb" command creates a new Amazon S3 bucket with the specified name. Here's a breakdown of the different parts of the command:

- "aws" is the CLI (command-line interface) for interacting with Amazon Web Services.
- "s3" refers to the S3 service within AWS, which stands for Simple Storage Service.
- "mb" stands for "make bucket", which is the action that will be taken with this command.
- The name of the bucket will need to be specified after the command. This should be a unique name that adheres to S3 naming rules (such as using only lowercase letters, numbers, and dashes, and not starting or ending with a dash). 

Example usage:

`aws s3 mb s3://my-new-bucket-name`

This command will create a new S3 bucket called "my-new-bucket-name". If successful, the command should return a message confirming that the bucket was created. 

## tldr 
 
> Create S3 buckets.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3/mb.html>.

- Create an S3 bucket:

`aws s3 mb s3://{{bucket_name}}`

- Create an S3 bucket in a specific region:

`aws s3 mb s3://{{bucket_name}} --region {{region}}`

- Display help:

`aws s3 mb help`
