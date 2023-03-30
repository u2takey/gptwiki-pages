# theHarvester 
## chatgpt 
theHarvester is a command-line tool used for collecting information from various public sources about a target domain, email address, or username. It is used mainly by pentesters, security researchers, and cybersecurity professionals to discover potential vulnerabilities or attack vectors that could be used by attackers to gain unauthorized access to a system or data.

theHarvester supports different sources such as Google, Bing, LinkedIn, and PGP key servers. By using this tool, an analyst can retrieve the following types of data:

- Email addresses associated with the target domain
- Hostnames found in search engine results pages (SERP)
- List of employees associated with a company
- Open ports of the target system
- Subdomains of the target domain

Using theHarvester is quite easy. Once the tool is installed, the following command can be used:

theharvester -d target.com -l 500 -b google

The above command will search for email addresses associated with target.com domain using Google, and at most 500 possible email addresses will be returned.

Here is a brief explanation of each option used in the above command:

- -d: Target domain.
- -l: Limiter for search results. It specifies the maximum number of results returned by the search engine.
- -b: Source to be used for the search. In this case, Google is used. Other sources can be used such as Bing, LinkedIn, or PGP key servers, etc.

Overall, theHarvester is a powerful reconnaissance tool, which if used properly can help in identifying key information or weaknesses in a target system or organization. 

## tldr 
 
> A tool designed to be used in the early stages of a penetration test.
> More information: <https://github.com/laramies/theHarvester>.

- Gather information on a domain using Google:

`theHarvester --domain {{domain_name}} --source google`

- Gather information on a domain using multiple sources:

`theHarvester --domain {{domain_name}} --source {{google,bing,crtsh}}`

- Change the limit of results to work with:

`theHarvester --domain {{domain_name}} --source {{google}} --limit {{200}}`

- Save the output to two files in XML and HTML format:

`theHarvester --domain {{domain_name}} --source {{google}} --file {{output_file_name}}`

- Output all available options:

`theHarvester --help`
