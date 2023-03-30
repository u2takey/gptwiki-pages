# aws pricing 
## chatgpt 
The command "aws pricing" is used to access the Amazon Web Services (AWS) Pricing API, which provides access to AWS pricing data. 

When you run "aws pricing", you will see a list of available commands, which includes "describe-services", "get-attribute-values", "get-products", and "help". 

- "describe-services" allows you to view the services available in the Pricing API.
- "get-attribute-values" allows you to retrieve a list of attribute values for a specific service.
- "get-products" allows you to retrieve the pricing data for a specific product or service.
- "help" provides further assistance and examples of how to use the Pricing API.

This command can also be used in conjunction with other AWS CLI commands to automate pricing-related tasks, such as checking the cost of running specific instances or services. 

## tldr 
 
> Query services, products, and pricing information from Amazon Web Services.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/pricing/>.

- List service codes of a specific region:

`aws pricing describe-services --region {{us-east-1}}`

- List attributes for a given service code in a specific region:

`aws pricing describe-services --service-code {{AmazonEC2}} --region {{us-east-1}}`

- Print pricing information for a service code in a specific region:

`aws pricing get-products --service-code {{AmazonEC2}} --region {{us-east-1}}`

- List values for a specific attribute for a service code in a specific region:

`aws pricing get-attribute-values --service-code {{AmazonEC2}} --attribute-name {{instanceType}} --region {{us-east-1}}`

- Print pricing information for a service code using filters for instance type and location:

`aws pricing get-products --service-code {{AmazonEC2}} --filters "{{Type=TERM_MATCH,Field=instanceType,Value=m5.xlarge}}" "{{Type=TERM_MATCH,Field=location,Value=US East (N. Virginia)}}" --region {{us-east-1}}`
