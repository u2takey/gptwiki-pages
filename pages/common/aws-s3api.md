# aws s3api 
## chatgpt 
The `aws s3api` command is one of the Amazon Web Services Command Line Interface (CLI) commands used to interact with the Simple Storage Service (S3) API. It allows users to perform administrative tasks such as creating, modifying, or deleting S3 buckets and objects.

`aws s3api` provides a low-level interface for interacting with S3 services, as it communicates directly with the S3 API without any additional abstraction layer. This makes it a powerful tool with a wide range of functions that can be used to manage objects and buckets in an S3 environment.

Here are some of the common sub-commands that can be used with `aws s3api`:

- `create-bucket`:  Creates a new S3 bucket in a specified region.
- `put-object`: Adds or replaces an object in an S3 bucket. This command can be used to upload a file to an S3 bucket.
- `get-object`: Retrieves an object from an S3 bucket and saves it locally.
- `list-buckets`: Lists all buckets owned by the authenticated user.
- `list-objects`: Lists all objects within an S3 bucket.
- `delete-object`: Deletes an object from an S3 bucket.

To use `aws s3api` command, users must have valid AWS credentials and be authorized to access the S3 resources. The command requires knowledge of the S3 API and syntax of various sub-commands. It can be executed in the terminal or in scripts. 

## tldr 
 
> Create and delete Amazon S3 buckets and edit bucket properties.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3api/index.html>.

- Create bucket in a specific region:

`aws s3api create-bucket --bucket {{bucket_name}} --region {{region}} --create-bucket-configuration LocationConstraint={{region}}`

- Delete a bucket:

`aws s3api delete-bucket --bucket {{bucket_name}}`

- List buckets:

`aws s3api list-buckets`

- List the objects inside of a bucket and only show each object's key and size:

`aws s3api list-objects --bucket {{bucket_name}} --query '{{Contents[].{Key: Key, Size: Size}}}'`

- Add an object to a bucket:

`aws s3api put-object --bucket {{bucket_name}} --key {{object_key}} --body {{path/to/file}}`

- Download object from a bucket (The output file is always the last argument):

`aws s3api get-object --bucket {{bucket_name}} --key {{object_key}} {{path/to/output_file}}`

- Apply an Amazon S3 bucket policy to a specified bucket:

`aws s3api put-bucket-policy --bucket {{bucket_name}} --policy file://{{path/to/bucket_policy.json}}`

- Download the Amazon S3 bucket policy from a specified bucket:

`aws s3api get-bucket-policy --bucket {{bucket_name}} --query Policy --output {{json|table|text|yaml|yaml-stream}} > {{path/to/bucket_policy}}`
