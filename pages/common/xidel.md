# xidel 
## chatgpt 
xidel is a command line tool that allows users to extract and manipulate data from HTML/XML documents and JSON or plain text files. 

The basic syntax for using xidel is as follows:

xidel [input-file] [options] [query]

[input-file] - This is the input file that xidel will process. It can be an HTML, XML, JSON, or plain text file.

[options] - These are optional flags that modify how xidel processes the input file. For example, -s specifies that the input file is a shell command rather than a file, -q specifies that the output should be in quiet mode, and -f specifies a configuration file for xidel.

[query] - This is the query that xidel will use to extract data from the input file. The query language used by xidel is based on XPath and allows users to select elements or attributes based on certain criteria.

Some examples of xidel commands include:

xidel input.html -s '#submit-button' - This command would select the submit button on an HTML page with the id of "submit-button."

xidel input.json '[?price > 100]' - This command would select all objects in the input JSON file where the "price" attribute is greater than 100.

xidel input.xml -e '//book[author="Stephen King"]/title' - This command would select the titles of all books in an XML file where the author is "Stephen King."

Overall, xidel is a versatile and powerful command line tool that can be used to easily extract and manipulate data from various types of documents. 

## tldr 
 
> Download and extract data from HTML/XML pages as well as JSON APIs.
> More information: <https://www.videlibri.de/xidel.html>.

- Print all URLs found by a Google search:

`xidel {{https://www.google.com/search?q=test}} --extract "//a/extract(@href, 'url[?]q=([^&]+)&', 1)[. != '']"`

- Print the title of all pages found by a Google search and download them:

`xidel {{https://www.google.com/search?q=test}} --follow "{{//a/extract(@href, 'url[?]q=([^&]+)&', 1)[. != '']}}" --extract {{//title}} --download {{'{$host}/'}}`

- Follow all links on a page and print the titles, with XPath:

`xidel {{https://example.org}} --follow {{//a}} --extract {{//title}}`

- Follow all links on a page and print the titles, with CSS selectors:

`xidel {{https://example.org}} --follow "{{css('a')}}" --css {{title}}`

- Follow all links on a page and print the titles, with pattern matching:

`xidel {{https://example.org}} --follow "{{<a>{.}</a>*}}" --extract "{{<title>{.}</title>}}"`

- Read the pattern from example.xml (which will also check if the element containing "ood" is there, and fail otherwise):

`xidel {{path/to/example.xml}} --extract "{{<x><foo>ood</foo><bar>{.}</bar></x>}}"`

- Print all newest Stack Overflow questions with title and URL using pattern matching on their RSS feed:

`xidel {{http://stackoverflow.com/feeds}} --extract "{{<entry><title>{title:=.}</title><link>{uri:=@href}</link></entry>+}}"`

- Check for unread Reddit mail, Webscraping, combining CSS, XPath, JSONiq, and automatically form evaluation:

`xidel {{https://reddit.com}} --follow "{{form(css('form.login-form')[1], {'user': '$your_username', 'passwd': '$your_password'})}}" --extract "{{css('#mail')/@title}}"`
