# aws glue 
## chatgpt 
AWS Glue is a fully-managed extract, transform, and load (ETL) service that makes it easy for customers to prepare and load their data for analytics. It is a serverless data integration and transformation service that makes it easy to to discover, prepare, and combine data for analytical purposes.

The AWS Glue command-line interface (CLI) provides you with an executable that you can use to automate the creation and administration of AWS Glue resources. You can use the AWS Glue CLI to create, manage, and delete AWS Glue resources such as connections, crawlers, jobs, and triggers. 

Some common AWS Glue commands include:

- create-crawler: Creates a crawler to extract metadata from a data source and create or update AWS Glue metadata tables based on that metadata.
- create-job: Creates a new ETL job in AWS Glue.
- start-crawler: Starts a crawler to extract metadata from a data source and create or update AWS Glue metadata tables based on that metadata.
- start-job-run: Starts a new run of an AWS Glue ETL job.
- create-trigger: Creates a trigger that starts an ETL job when a specified event occurs.
- get-crawler-metrics: Retrieves the number of objects and the size of data that ETL crawlers have extracted; the number of tables that ETL crawlers have discovered; and the time ETL crawlers took to extract metadata from data sources.

By using the AWS Glue CLI, you can automate your ETL workflows and integrate your data from various sources into a single, consolidated data store for analysis. 

## tldr 
 
> CLI for AWS Glue.
> Defines the public endpoint for the AWS Glue service.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/glue/>.

- List jobs:

`aws glue list-jobs`

- Start a job:

`aws glue start-job-run --job-name {{job_name}}`

- Start running a workflow:

`aws glue start-workflow-run --name {{workflow_name}}`

- List triggers:

`aws glue list-triggers`

- Start a trigger:

`aws glue start-trigger --name {{trigger_name}}`

- Create a dev endpoint:

`aws glue create-dev-endpoint --endpoint-name {{name}} --role-arn {{role_arn_used_by_endpoint}}`
