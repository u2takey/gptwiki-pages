# xmllint 
## chatgpt 
The `xmllint` command is a widely-used tool for validating and parsing XML documents. It is used by developers, software testers, and other IT professionals to verify the syntax and structure of XML files, troubleshoot issues with XML-based applications, and perform various other tasks related to XML processing.

Here are some of the key features and capabilities of the `xmllint` command:

1. Syntax validation: The tool can check whether an XML file adheres to the XML syntax rules, such as the correct use of tags, attributes, and entities.

2. Structural validation: `xmllint` can also verify whether an XML file conforms to a specific schema or document type definition (DTD). This is useful for ensuring that the XML file meets specific requirements, such as the order of elements, the data types of attributes, and so on.

3. Well-formedness checking: In addition to validating the syntax and structure of an XML file, `xmllint` can also check whether the file is "well-formed." This means that the file follows all of the rules of XML, including having a single root element and properly nested elements.

4. XPath querying: `xmllint` supports XPath, a language used to select elements and attributes from an XML document based on their properties or values. With `xmllint`, you can run XPath queries against an XML file to extract specific information.

5. Formatting and transformation: The tool can be used to format an XML file for easier readability, such as by indenting elements and attributes. It can also be used to transform XML documents into other formats, such as HTML, using XSLT (eXtensible Stylesheet Language Transformations).

In summary, `xmllint` is a versatile and powerful command-line tool that is essential for working with XML files in many different contexts. 

## tldr 
 
> XML parser and linter that supports XPath, a syntax for navigating XML trees.
> More information: <https://manned.org/xmllint>.

- Return all nodes (tags) named "foo":

`xmllint --xpath "//{{foo}}" {{source_file.xml}}`

- Return the contents of the first node named "foo" as a string:

`xmllint --xpath "string(//{{foo}})" {{source_file.xml}}`

- Return the href attribute of the second anchor element in an HTML file:

`xmllint --html --xpath "string(//a[2]/@href)" webpage.xhtml`

- Return human-readable (indented) XML from file:

`xmllint --format {{source_file.xml}}`

- Check that an XML file meets the requirements of its DOCTYPE declaration:

`xmllint --valid {{source_file.xml}}`

- Validate XML against DTD schema hosted online:

`xmllint --dtdvalid {{URL}} {{source_file.xml}}`
