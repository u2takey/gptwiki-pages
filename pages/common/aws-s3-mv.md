# aws s3 mv 
## chatgpt 
The AWS S3 mv command is used to move or rename files and directories in Amazon S3 buckets. The syntax of the command is as follows:

aws s3 mv s3://source/filename.ext s3://destination/filename.ext

Here, 'source' and 'destination' are the S3 bucket paths. The 'filename.ext' is the file or object name that is to be moved or renamed.

The 'mv' command essentially performs two operations - copy and delete. It copies the file from the source bucket to the destination bucket and deletes the file from the source bucket, thereby moving it to the specified location. If the source and destination buckets are in the same region, the copy operation is optimized and faster.

The 'mv' command can also be used to rename a file or directory in the same bucket. In this case, the source and destination bucket paths are the same. The syntax for renaming a file is as follows:

aws s3 mv s3://bucket/oldfilename.ext s3://bucket/newfilename.ext

Here, 'oldfilename.ext' is the original file name, and 'newfilename.ext' is the new file name.

Additional options can be provided with the 'mv' command to customize its behavior, such as specifying ACLs, encryption, and metadata. The command can also be used in combination with AWS Identity and Access Management (IAM) policies to provide granular access control. 

## tldr 
 
> Move local files or S3 objects to another location locally or in S3.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3/mv.html>.

- Move a file from local to a specified bucket:

`aws s3 mv {{path/to/local_file}} s3://{{bucket_name}}/{{path/to/remote_file}}`

- Move a specific S3 object into another bucket:

`aws s3 mv s3://{{bucket_name1}}/{{path/to/file}} s3://{{bucket_name2}}/{{path/to/target}}`

- Move a specific S3 object into another bucket keeping the original name:

`aws s3 mv s3://{{bucket_name1}}/{{path/to/file}} s3://{{bucket_name2}}`

- Display help:

`aws s3 mv help`
