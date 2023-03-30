# aws kinesis 
## chatgpt 
AWS Kinesis is a managed streaming data service provided by Amazon Web Services (AWS) that enables real-time processing of streaming data at scale. It simplifies the process of collecting and analyzing large volumes of streaming data from a variety of sources, including IoT devices, social media networks, and mobile applications.

The basic syntax for the AWS Kinesis command is:

aws kinesis [parameters]

This command allows users to interact with the Kinesis service from the command line interface (CLI) by specifying parameters that define the actions to be taken. Some of the commonly used parameters include:

- create-stream: Create a new Kinesis stream with the specified name and number of shards.
- list-streams: List all Kinesis streams in the AWS account.
- describe-stream: Get information about a specific Kinesis stream, such as the number of shards, the status of the stream, and the associated AWS resources.
- put-record: Add a single data record to a specified Kinesis stream.
- get-records: Retrieve the data records from a specified shard in a Kinesis stream.
- delete-stream: Delete a specified Kinesis stream and all associated data. 

Additionally, the aws kinesis command can be extended with other AWS services such as AWS Lambda, AWS CloudWatch, and AWS IAM to create more complex workflows for processing streaming data. 

## tldr 
 
> Official AWS CLI for Amazon Kinesis streaming data services.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/kinesis/index.html#cli-aws-kinesis>.

- Show all streams in the account:

`aws kinesis list-streams`

- Write one record to a Kinesis stream:

`aws kinesis put-record --stream-name {{name}} --partition-key {{key}} --data {{base64_encoded_message}}`

- Write a record to a Kinesis stream with inline base64 encoding:

`aws kinesis put-record --stream-name {{name}} --partition-key {{key}} --data "$( echo "{{my raw message}}" | base64 )"`

- List the shards available on a stream:

`aws kinesis list-shards --stream-name {{name}}`

- Get a shard iterator for reading from the oldest message in a stream's shard:

`aws kinesis get-shard-iterator --shard-iterator-type TRIM_HORIZON --stream-name {{name}} --shard-id {{id}}`

- Read records from a shard, using a shard iterator:

`aws kinesis get-records --shard-iterator {{iterator}}`
