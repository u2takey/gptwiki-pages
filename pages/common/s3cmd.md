# s3cmd 
## chatgpt 
S3cmd is a command-line tool for interacting with Amazon S3 (Simple Storage Service) and other S3-compatible storage services like Ceph, Minio, etc. This command-line tool provides an easy-to-use interface for uploading, downloading, and managing objects (files) on S3 and S3-compatible storage services.

Here are some of the common commands that can be used with s3cmd:

1. s3cmd ls:
This command lists all the objects in the bucket.

2. s3cmd mb:
This command is used to create a new bucket.

3. s3cmd rb:
This command is used to delete a bucket.

4. s3cmd put:
This command is used to upload objects to S3.

5. s3cmd get:
This command is used to download objects from S3.

6. s3cmd cp:
This command is used to copy objects from one bucket location to another.

7. s3cmd mv:
This command is used to move objects from one bucket location to another.

8. s3cmd sync:
This command is used to synchronize a local directory with an S3 bucket.

9. s3cmd du:
This command is used to get the total size of a bucket.

10. s3cmd del:
This command is used to delete objects from S3.

In summary, s3cmd provides an easy and efficient way to interact with Amazon S3 and other S3-compatible storage services using the command line. 

## tldr 
 
> Command line tool and client for uploading, retrieving and managing data in S3 compatible object storage.
> More information: <https://s3tools.org/s3cmd>.

- Invoke configuration/reconfiguration tool:

`s3cmd --configure`

- List Buckets/Folders/Objects:

`s3cmd ls s3://{{bucket|path/to/file}}`

- Create Bucket/Folder:

`s3cmd mb s3://{{bucket}}`

- Download a specific file from a bucket:

`s3cmd get s3://{{bucket_name}}/{{path/to/file}} {{path/to/local_file}}`

- Upload a file to a bucket:

`s3cmd put {{local_file}} s3://{{bucket}}/{{file}}`

- Move an object to a specific bucket location:

`s3cmd mv s3://{{src_bucket}}/{{src_object}} s3://{{dst_bucket}}/{{dst_object}}`

- Delete a specific object:

`s3cmd rm s3://{{bucket}}/{{object}}`
