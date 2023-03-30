# idnits 
## chatgpt 
The `idnits` command is a tool for checking and verifying Internet Drafts (I-Ds) for compliance with the document formatting requirements of the Internet Engineering Task Force (IETF). 

When an I-D is submitted to the IETF, it must conform to specific formatting requirements, such as proper use of language and grammar, appropriate categorization and organization of sections, and proper use of references and citations. The `idnits` tool is designed to check I-Ds for adherence to these requirements.

When the `idnits` command is executed, it analyzes the I-D file and generates a detailed report of any formatting or syntax errors that are detected. The report includes information on specific errors, as well as recommendations and guidelines for fixing the errors.

`idnits` is an important tool for helping IETF authors ensure that their documents meet the necessary formatting requirements and, as a result, have a better chance of being accepted and considered for publication. 

## tldr 
 
> Check internet-drafts for submission nits.
> Looks for violations of Section 2.1 and 2.2 of the requirements listed on <https://www.ietf.org/id-info/checklist>.
> More information: <https://tools.ietf.org/tools/idnits/>.

- Check a file for nits:

`idnits {{path/to/file.txt}}`

- Count nits without displaying them:

`idnits --nitcount {{path/to/file.txt}}`

- Show extra information about offending lines:

`idnits --verbose {{path/to/file.txt}}`

- Expect the specified year in the boilerplate instead of the current year:

`idnits --year {{2021}} {{path/to/file.txt}}`

- Assume the document is of the specified status:

`idnits --doctype {{standard|informational|experimental|bcp|ps|ds}} {{path/to/file.txt}}`
