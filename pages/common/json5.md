# json5 
## chatgpt 
`json5` is a command line tool used to parse, validate, and manipulate JSON data. It is an extension of the JSON format that adds support for comments, trailing commas, and more flexible syntax for defining objects and arrays.

When run in the command line and given a JSON5 file as input, `json5` will attempt to parse and validate the data in the file. If the file contains an error, `json5` will display an error message detailing the issue with the data.

`json5` can also be used to convert JSON5 data into regular JSON format, using the `--json` flag. This can be useful when working with systems that only support JSON, as the JSON5 format is not always compatible.

Overall, `json5` is a useful tool for working with JSON data, especially for developers who prefer a more flexible syntax and the ability to add comments to their data. 

## tldr 
 
> A command-line tool for converting JSON5 files to JSON.
> More information: <https://json5.org>.

- Convert JSON5 `stdin` to JSON `stdout`:

`echo {{input}} | json5`

- Convert a JSON5 file to JSON and output to `stdout`:

`json5 {{path/to/input_file.json5}}`

- Convert a JSON5 file to the specified JSON file:

`json5 {{path/to/input_file.json5}} --out-file {{path/to/output_file.json}}`

- Validate a JSON5 file:

`json5 {{path/to/input_file.json5}} --validate`

- Specify the number of spaces to indent by (or "t" for tabs):

`json5 --space {{indent_amount}}`

- View available options:

`json5 --help`
