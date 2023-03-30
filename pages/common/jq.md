# jq 
## chatgpt 
The `jq` command is a deep-dive tool for manipulating and processing JSON data. It is primarily used for parsing, filtering, and transforming JSON objects and arrays.

Here are some of the common use cases for the `jq` command:

1. Formatting JSON data: `jq . input.json` will pretty-print the contents of the `input.json` file.

2. Selecting specific fields: `jq '.foo.bar' input.json` will extract the `bar` field of the `foo` object in the `input.json` file.

3. Filtering JSON data: `jq '.[] | select(.age > 30)' input.json` will filter out all objects in a JSON array where the `age` field is less than or equal to 30.

4. Transforming JSON data: `jq '.name = "John Doe"' input.json` will update the `name` field of the root object to `John Doe`.

5. Combining multiple JSON files: `jq -s 'add' file1.json file2.json` will combine the contents of `file1.json` and `file2.json` into a single JSON object.

The `jq` command is a powerful and flexible tool for working with JSON data, and can be a great option for performing complex data manipulations or transformations. 

## tldr 
 
> A command-line JSON processor that uses a domain-specific language.
> More information: <https://stedolan.github.io/jq/manual/>.

- Execute a specific expression (print a colored and formatted json):

`{{cat path/to/file.json}} | jq '.'`

- Execute a specific script:

`{{cat path/to/file.json}} | jq --from-file {{path/to/script.jq}}`

- Pass specific arguments:

`{{cat path/to/file.json}} | jq {{--arg "name1" "value1" --arg "name2" "value2" ...}} '{{. + $ARGS.named}}'`

- Print specific keys:

`{{cat path/to/file.json}} | jq '{{.key1, .key2, ...}}'`

- Print specific array items:

`{{cat path/to/file.json}} | jq '{{.[index1], .[index2], ...}}'`

- Print all array items/object keys:

`{{cat path/to/file.json}} | jq '.[]'`

- Add/remove specific keys:

`{{cat path/to/file.json}} | jq '. {{+|-}} {{{"key1": "value1", "key2": "value2", ...}}}'`
