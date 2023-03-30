# xml elements 
## chatgpt 
XML elements are the building blocks of an XML document. An XML element consists of a start-tag, the content of the element, and an end-tag. 

The start-tag of an XML element denotes the start of the element and is enclosed in angle brackets < >. The name of the element appears after the opening angle bracket. For example, <book> is the start-tag of an element named 'book'.

The end-tag of an XML element denotes the end of the element and is also enclosed in angle brackets. The end-tag includes a forward slash / after the opening angle bracket, followed by the element name. For example, </book> is the end-tag for the 'book' element.

The content of an XML element is the information that appears between the start-tag and the end-tag. For example, <book>Harry Potter and the Philosopher's Stone</book> is an XML element where the content is 'Harry Potter and the Philosopher's Stone'.

In summary, XML elements are defined by a start-tag, content, and an end-tag, and they encapsulate data within an XML document. 

## tldr 
 
> Extract elements and display the structure of an XML document.
> More information: <http://xmlstar.sourceforge.net/docs.php>.

- Extract elements from an XML document (producing XPATH expressions):

`xml elements {{path/to/input.xml|URI}} > {{path/to/elements.xpath}}`

- Extract elements and their attributes from an XML document:

`xml elements -a {{path/to/input.xml|URI}} > {{path/to/elements.xpath}}`

- Extract elements and their attributes and values from an XML document:

`xml elements -v {{path/to/input.xml|URI}} > {{path/to/elements.xpath}}`

- Print sorted unique elements from an XML document to see its structure:

`xml elements -u {{path/to/input.xml|URI}}`

- Print sorted unique elements from an XML document up to a depth of 3:

`xml elements -d{{3}} {{path/to/input.xml|URI}}`

- Display help for the `elements` subcommand:

`xml elements --help`
