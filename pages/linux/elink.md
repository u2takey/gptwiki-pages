# elink 
## chatgpt 
The elink command is not a standard command found in most operating systems. It is possible that the command you are referring to is specific to a particular software or application.

In general, the prefix "e" may refer to electronic or internet-related functions, while "link" usually refers to connecting or combining different elements.

Some applications or software that may have an elink command include:

1. E-Link for MS Publisher: This is an add-on for Microsoft Publisher that allows users to create interactive publications that can be linked to other online content.

2. E-Link Gateway: This is a software package that helps organizations to integrate different types of electronic documents and files into a common platform.

3. Elink.io: This is a web service that allows users to create and share links to different types of web content, including articles, videos, and images.

Without more information about the specific context and purpose of the elink command, it is difficult to provide further details about its function. 

## tldr 
 
> Look up precomputed neighbors within a database, or find associated records in other databases.
> It is part of the `edirect` package.
> More information: <https://www.ncbi.nlm.nih.gov/books/NBK179288/>.

- Search pubmed then find related sequences:

`esearch -db pubmed -query "{{selective serotonin reuptake inhibitor}}" | elink -target nuccore`

- Search nucleotide then find related biosamples:

`esearch -db nuccore -query "{{insulin [PROT] AND rodents [ORGN]}}" | elink -target biosample`
