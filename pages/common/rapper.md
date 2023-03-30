# rapper 
## chatgpt 
The command "rapper" is a command-line utility tool used to parse and generate metadata for RDF (Resource Description Framework) files in various formats such as RDF/XML, Turtle, and N-Triples. The tool is part of the Raptor RDF Syntax Library, which is a robust library for working with RDF data.

The "rapper" command allows users to convert RDF files from one format to another format, validate the RDF syntax, and generate metadata for the RDF data. The command takes several options and arguments that can be used to customize the output and behavior of the tool.

Some of the most commonly used options of the "rapper" command include:

- "-i" or "--input-format": This option specifies the input format of the RDF file. The format can be auto-detected by default, or it can be explicitly specified using this option. Example: "rapper -i turtle file.rdf".

- "-o" or "--output-format": This option specifies the output format of the RDF file. The format can be auto-detected by default, or it can be explicitly specified using this option. Example: "rapper -o rdfxml file.ttl".

- "-c" or "--count": This option specifies the number of triples in the RDF file to be displayed. Example: "rapper -c file.rdf".

- "-l" or "--limit": This option specifies the maximum number of errors or warnings to be displayed during the parsing of the RDF file. Example: "rapper -l 10 file.rdf".

- "-v" or "--verbose": This option enables verbose output, which provides more detailed information about the operations performed by the tool. Example: "rapper -v file.rdf".

In summary, "rapper" is a powerful command-line tool that allows users to work with RDF data and metadata in various formats. It can be used for performing parsing, conversion, and validation operations on RDF files. 

## tldr 
 
> The Raptor RDF parsing utility.
> Part of the Raptor RDF Syntax Library.
> More information: <http://librdf.org/raptor/rapper.html>.

- Convert an RDF/XML document to Turtle:

`rapper -i rdfxml -o turtle {{path/to/file}}`

- Count the number of triples in a Turtle file:

`rapper -i turtle -c {{path/to/file}}`
