# aws route53 
## chatgpt 
aws route53 is a command-line tool provided by Amazon Web Services (AWS) for managing domain name system (DNS) records and settings hosted in Amazon Route 53, a highly available and scalable cloud DNS service. The command offers various sub-commands that can be used for specific operations related to Route 53.

Some of the commonly used sub-commands and their descriptions are:

- change-resource-record-sets: Used to create, modify, or delete DNS records for a hosted zone in Route 53.
- create-reusable-delegation-set: Used to create a reusable delegation set in Route 53, which can be used to associate multiple hosted zones with a set of name servers.
- create-hosted-zone: Used to create a new hosted zone in Route 53.
- delete-hosted-zone: Used to delete a hosted zone in Route 53.
- list-hosted-zones: Used to list all the hosted zones in a Route 53 account.
- list-resource-record-sets: Used to list all the DNS records for a specific hosted zone.

To use the aws route53 command, you need to have AWS CLI installed on your system and configured with your AWS account credentials. Once you have done that, you can run the desired sub-command with the required parameters and options to manage your Route 53 resources. 

## tldr 
 
> CLI for AWS Route53 - Route 53 is a highly available and scalable Domain Name System (DNS) web service.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/route53/index.html>.

- List all hosted zones, private and public:

`aws route53 list-hosted-zones`

- Show all records in a zone:

`aws route53 list-resource-record-sets --hosted-zone-id {{zone_id}}`

- Create a new, public zone using a request identifier to retry the operation safely:

`aws route53 create-hosted-zone --name {{name}} --caller-reference {{request_identifier}}`

- Delete a zone (if the zone has non-defaults SOA and NS records the command will fail):

`aws route53 delete-hosted-zone --id {{zone_id}}`

- Test DNS resolving by Amazon servers of a given zone:

`aws route53 test-dns-answer --hosted-zone-id {{zone_id}}  --record-name {{name}} --record-type {{type}}`
