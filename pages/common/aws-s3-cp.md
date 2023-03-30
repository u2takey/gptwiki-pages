# aws s3 cp 
## chatgpt 
The "aws s3 cp" command is a command-line interface (CLI) command used to copy files or directories from a local source to an Amazon Web Services (AWS) Simple Storage Service (S3) bucket or vice versa.

The "aws" command is used to interact with AWS services from the command line, and "s3" is the AWS service used to store and retrieve files.

The "cp" command is used to perform a copy operation, wherein the source file(s) or directory is copied to the specified S3 bucket or local location.

The syntax for the command is as follows:
aws s3 cp <source> <destination> [options]

- <source> refers to the path to the local file(s) or directory to be copied, or the S3 object to be copied.
- <destination> refers to the location to which the file or directory will be copied, either a local directory or S3 bucket/path.
- [options] can be used to add additional parameters to the command, such as the "--recursive" parameter for copying a directory or the "--acl" parameter to set access control lists for the copied file or directory.

One example of using the command is as follows:

aws s3 cp ~/Desktop/my_file.txt s3://my-bucket/

This command would copy the file "my_file.txt", located on the user's desktop, to an S3 bucket called "my-bucket". 

## tldr 
 
> Copy local files or S3 objects to another location locally or in S3.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3/cp.html>.

- Copy a file from local to a specific bucket:

`aws s3 cp {{path/to/file}} s3://{{bucket_name}}/{{path/to/remote_file}}`

- Copy a specific S3 object into another bucket:

`aws s3 cp s3://{{bucket_name1}}/{{path/to/file}} s3://{{bucket_name2}}/{{path/to/target}}`

- Copy a specific S3 object into another bucket keeping the original name:

`aws s3 cp s3://{{bucket_name1}}/{{path/to/file}} s3://{{bucket_name2}}`

- Copy S3 objects to a local directory recursively:

`aws s3 cp s3://{{bucket_name}} . --recursive`

- Display help:

`aws s3 cp help`
