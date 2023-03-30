# gsutil 
## chatgpt 
The command "gsutil" is part of the Google Cloud Storage utility. It is a command-line tool that allows users to interact with Google Cloud Storage from a terminal or command prompt.

Here's a brief rundown of some of the key features of gsutil:

1. Bucket and object management: With gsutil, users can create, delete, and modify storage buckets and their contained objects.

2. Data transfer and syncing: Users can upload and download files to and from their cloud storage, as well as sync files to keep their local and cloud environments up-to-date.

3. Access control: gsutil provides granular access controls for storage buckets and objects, allowing users to grant or revoke permissions as needed.

4. Batch operations: The tool is designed to handle large-scale operations with ease, allowing you to work with thousands of files at once.

Overall, gsutil is a powerful tool for managing cloud storage in a command-line environment. Whether you're working with a small personal project or managing enterprise-scale data storage, gsutil can help you get the job done quickly and efficiently. 

## tldr 
 
> The gsutil CLI lets you access Google Cloud Storage from the command line.
> You can use gsutil to do a wide range of bucket and object management tasks.
> More information: <https://cloud.google.com/storage/docs/gsutil>.

- List all buckets in a project you are logged into:

`gsutil ls`

- List the objects in a bucket:

`gsutil ls -r 'gs://{{bucket_name}}/{{prefix}}**'`

- Download an object from a bucket:

`gsutil cp gs://{{bucket_name}}/{{object_name}} {{path/to/save_location}}`

- Upload an object to a bucket:

`gsutil cp {{object_location}} gs://{{destination_bucket_name}}/`

- Rename or move objects in a bucket:

`gsutil mv gs://{{bucket_name}}/{{old_object_name}} gs://{{bucket_name}}/{{new_object_name}}`

- Create a new bucket in the project you are logged into:

`gsutil mb gs://{{bucket_name}}`

- Delete a bucket and remove all the objects in it:

`gsutil rm -r gs://{{bucket_name}}`
