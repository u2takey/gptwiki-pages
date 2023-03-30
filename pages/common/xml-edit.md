# xml edit 
## chatgpt 
As an AI language model, I cannot provide exact information on what "xml edit" command does since it is not a specific command in any particular context. However, I could provide an explanation on what XML and editing XML files generally means.

XML (Extensible Markup Language) is a markup language used to store and transport data in a structured format. XML files contain tags that define the structure and content of the data stored in the file. Editing XML files usually involves modifying the tags and the data associated with them to add or remove information, update existing data or restructure the layout of the file.

There are various XML editors and parsers that allow developers and users to edit XML files. These tools enable users to validate the structure of the XML file, modify the content, and save the changes made to the file. Some editors also provide features such as syntax highlighting, auto-completion, and debugging which help users to work with XML files more efficiently.

In summary, the "xml edit" command is not a specific command, but editing XML files involves modifying the tags and data associated with them to manipulate the content stored in an XML file. 

## tldr 
 
> Edit an XML document.
> More information: <http://xmlstar.sourceforge.net/docs.php>.

- Delete elements matching an XPATH from an XML document:

`xml edit --delete "{{XPATH1}}" {{path/to/input.xml|URI}}`

- Move an element node of an XML document from XPATH1 to XPATH2:

`xml edit --move "{{XPATH1}}" "{{XPATH2}}" {{path/to/input.xml|URI}}`

- Rename all attributes named "id" to "ID":

`xml edit --rename "{{//*/@id}}" -v "{{ID}}" {{path/to/input.xml|URI}}`

- Rename sub-elements of the element "table" that are named "rec" to "record":

`xml edit --rename "{{/xml/table/rec}}" -v "{{record}}" {{path/to/input.xml|URI}}`

- Update the XML table record with "id=3" to the value "id=5":

`xml edit --update "{{xml/table/rec[@id=3]/@id}}" -v {{5}} {{path/to/input.xml|URI}}`

- Display help for the `edit` subcommand:

`xml edit --help`
