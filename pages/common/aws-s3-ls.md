# aws s3 ls 
## chatgpt 
The command "aws s3 ls" is used to list the contents of an Amazon S3 bucket. Here is an explanation of each part of the command:

- "aws" is the command line interface for accessing Amazon Web Services (AWS).
- "s3" refers to Amazon Simple Storage Service (S3), which is a cloud-based storage service offered by AWS.
- "ls" is a shorthand for "list," which instructs the AWS CLI to list the contents of the specified S3 bucket.

When you run the command "aws s3 ls," the CLI will list the names of the objects (files) in the default S3 bucket in the format of "LastModified Date Time", "Size of the object in bytes" (in form of abbreviation B, KB, MB, GB, etc.) and "Object Key (the name of the object)". 

You can specify the name of a specific bucket by adding the name of the bucket to the end of the command, like this: "aws s3 ls example-bucket". This will list the objects in the "example-bucket" S3 bucket. 

Overall, the "aws s3 ls" command is a useful way to quickly view the objects in an S3 bucket from the command line. 

## tldr 
 
> List AWS S3 buckets, folders (prefixes), and files (objects).
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3/ls.html>.

- List all buckets:

`aws s3 ls`

- List files and folders in the root of a bucket (`s3://` is optional):

`aws s3 ls s3://{{bucket_name}}`

- List files and folders directly inside a directory:

`aws s3 ls {{bucket_name}}/{{path/to/directory}}/`

- List all files in a bucket:

`aws s3 ls --recursive {{bucket_name}}`

- List all files in a path with a given prefix:

`aws s3 ls --recursive {{bucket_name}}/{{path/to/directory/}}{{prefix}}`

- Display help:

`aws s3 ls help`
