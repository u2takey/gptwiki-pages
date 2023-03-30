# phpquery 
## chatgpt 
I'm sorry, but "phpquery" is not a valid or recognized command in the PHP programming language. 

However, there is a popular PHP library and tool called "PHPQuery" which is used to parse and manipulate HTML documents using CSS selectors (similar to jQuery in JavaScript). 

PHPQuery enables you to extract data from HTML web pages, modify the DOM structure, and even create new HTML elements. It makes working with HTML in PHP code much easier, simpler, and quicker. 

To use PHPQuery in your PHP application, you need to include its library file and initialized it by creating a new instance of the class with the HTML code you want to work with. Then, you can access and manipulate the HTML elements using various PHP methods and functions provided by the PHPQuery library. 

Here's an example of how to initialize PHPQuery with a URL:

```php
include('path/to/phpquery.php');
$doc = phpQuery::newDocumentFile('http://example.com');
```

This creates a new instance of the PHPQuery class, and loads the HTML code from 'http://example.com'. 

Then, you can use various methods to work with the HTML code, for example:

```php
$titles = $doc->find('title'); // find all <title> elements
echo count($titles); // outputs the number of <title> elements found
$title = $doc->find('title')->text(); // extract the text of the first <title> element
echo $title; // outputs the text of the first <title> element
```

These are just some basic examples of how you can use PHPQuery to manipulate HTML code. There are many more features and methods provided by the library for more advanced use cases. 

## tldr 
 
> PHP extension manager for Debian-based OSes.
> More information: <https://helpmanual.io/help/phpquery/>.

- List available PHP versions:

`sudo phpquery -V`

- List available SAPIs for PHP 7.3:

`sudo phpquery -v {{7.3}} -S`

- List enabled extensions for PHP 7.3 with the cli SAPI:

`sudo phpquery -v {{7.3}} -s {{cli}} -M`

- Check if the JSON extension is enabled for PHP 7.3 with the apache2 SAPI:

`sudo phpquery -v {{7.3}} -s {{apache2}} -m {{json}}`
