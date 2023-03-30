# nokogiri 
## chatgpt 
Nokogiri is a command-line tool used for parsing and manipulating HTML and XML documents in Ruby programming language. It is a Ruby Gem that provides a comprehensive set of features and capabilities for working with HTML and XML documents. 

Nokogiri provides various methods to navigate and manipulate HTML/XML documents, such as CSS selectors, XPath expressions, and DOM traversal. In addition, it also allows us to extract information from web pages, clean up the HTML/XML code, and modify the structure of documents.

To use Nokogiri in Ruby projects, you need to install it first via the command line. You can do so by running the following command:

```
gem install nokogiri
```

Once installed, you can use the Nokogiri command-line tool to perform various tasks such as parsing an HTML/XML document and performing operations on it. For example, to parse an HTML document using Nokogiri, you can run the following command:

```
nokogiri http://example.com/
```

This will parse the HTML document at the given URL and display it in the terminal. You can also chain various Nokogiri methods to perform more complex operations on the document.

Overall, Nokogiri is a powerful tool for working with HTML and XML documents in Ruby, and it provides a simple and efficient way to parse, manipulate, and extract information from these documents. 

## tldr 
 
> An HTML, XML, SAX and Reader parser.
> More information: <https://nokogiri.org>.

- Parse the contents of a URL or file:

`nokogiri {{url|path/to/file}}`

- Parse as a specific type:

`nokogiri {{url|path/to/file}} --type {{xml|html}}`

- Load a specific initialization file before parsing:

`nokogiri {{url|path/to/file}} -C {{path/to/config_file}}`

- Parse using a specific encoding:

`nokogiri {{url|path/to/file}} --encoding {{encoding}}`

- Validate using a RELAX NG file:

`nokogiri {{url|path/to/file}} --rng {{url|path/to/file}}`
