# in-toto-record 
## chatgpt 
The command "in-toto-record" is a tool provided by the in-toto framework. The in-toto framework is a set of tools and libraries designed to help ensure the integrity and security of software supply chains.

The "in-toto-record" command is used to create a record of the steps taken to produce a software artifact. This is done by creating a signed JSON file that contains metadata about the software and the steps that were taken to produce it. This information can be used to verify the integrity of the software and to ensure that it was produced in a secure and trustworthy manner.

The "in-toto-record" command takes several arguments:

1. --step-name: This argument specifies the name of the step being recorded. This should be a unique, descriptive name that identifies the step.

2. --key: This argument specifies the private key to use when signing the JSON file. This key should be kept secure and only used by trusted individuals.

3. --materials: This argument specifies a list of files or directories that were used as input to the step being recorded.

4. --products: This argument specifies a list of files or directories that were produced as output by the step being recorded.

5. --uxid: This argument specifies a unique identifier for the step being recorded. This can be used to track the step across different systems or software versions.

Once the "in-toto-record" command has been executed with the required arguments, it will create a signed JSON file that contains the metadata about the step that was recorded. This file can then be used to verify the integrity of the software artifact and to ensure that it was produced in a secure and trustworthy manner. 

## tldr 
 
> Create a signed link metadata file to provide evidence for supply chain steps.
> More information: <https://in-toto.readthedocs.io/en/latest/command-line-tools/in-toto-record.html>.

- Start the record (creates a preliminary link file):

`in-toto-record start -n {{edit-files}} -k {{path/to/key_file}} -m {{.}}`

- Stop the record (expects a preliminary link file):

`in-toto-record stop -n {{edit-files}} -k {{path/to/key_file}} -p {{.}}`
