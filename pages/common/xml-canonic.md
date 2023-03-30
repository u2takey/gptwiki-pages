# xml canonic 
## chatgpt 
The "xml canonic" command refers to the process of creating a canonical representation of an XML document. This means that the XML document is transformed into a standardized format that is the same regardless of the original formatting or order of elements in the document. This can be useful for ensuring consistency and compatibility between different systems that use XML.

The process of creating a canonical representation of an XML document typically involves several steps, such as removing comments and whitespace, sorting the attributes of each element in a specific order, and converting all attribute values to a standard format. The resulting document is then considered to be a canonical representation of the original XML document.

There are several tools and libraries available for performing XML canonicalization, such as the XML Security Library (XMLSec), Apache Santuario XML Security, and Canonical XML (C14N). These tools often provide a variety of options and customization settings to allow users to tailor the canonicalization process to their specific needs. 

## tldr 
 
> Make XML documents canonical.
> More information: <http://xmlstar.sourceforge.net/docs.php>.

- Make an XML document canonical, preserving comments:

`xml canonic {{path/to/input.xml|URI}} > {{path/to/output.xml}}`

- Make an XML document canonical, removing comments:

`xml canonic --without-comments {{path/to/input.xml|URI}} > {{path/to/output.xml}}`

- Make XML exclusively canonical, using an XPATH from a file, preserving comments:

`xml canonic --exc-with-comments {{path/to/input.xml|URI}} {{path/to/c14n.xpath}}`

- Display help for the `canonic` subcommand:

`xml canonic --help`
