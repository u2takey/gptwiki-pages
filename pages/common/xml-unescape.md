# xml unescape 
## chatgpt 
The command "xml unescape" is used to convert escaped XML characters back into their original form. In XML, certain characters, such as "<", ">", "&", "'", and """, have special meanings and need to be escaped in order to represent them as plain text. For example, "&lt;" represents the "<" symbol, and "&gt;" represents the ">" symbol.

The "xml unescape" command is used to reverse this process, taking escaped characters and converting them back to their original form. This can be useful if you need to analyze or modify XML data and want to see the data in its unescaped form.

To use the "xml unescape" command, you can typically specify a string or file containing the escaped XML data. The command will then output the unescaped XML data, with all escaped characters replaced by their original form. For example, if you have the string "&lt;title&gt;Hello, World!&lt;/title&gt;", the "xml unescape" command will convert it to "<title>Hello, World!</title>". 

## tldr 
 
> Unescape special XML characters, e.g. `&lt;a1&gt;` → `<a1>`.
> More information: <http://xmlstar.sourceforge.net/docs.php>.

- Unescape special XML characters from a string:

`xml unescape "{{&lt;a1&gt;}}"`

- Unescape special XML characters from `stdin`:

`echo  "{{&lt;a1&gt;}}" | xml unescape`

- Display help for the `unescape` subcommand:

`xml escape --help`
