# Test-Json 
## chatgpt 
The Test-Json command is a PowerShell cmdlet that is used to test whether a string or object is a valid JSON (JavaScript Object Notation) format or not. 

When executed, Test-Json cmdlet reads the input object, validates it against the JSON schema, and returns a Boolean value based on the validity of the JSON format. If the input object is in valid JSON format, the cmdlet returns "True". Otherwise, it returns "False".

Below is the Syntax of Test-Json command:

Test-Json [-InputObject] <Object> [<CommonParameters>]

The parameter "InputObject" specifies the object that needs to be validated as a JSON string. 

Here is an example of using Test-Json command:

PS C:\> $json_str = '{ "name": "John", "age": 30, "city": "New York"}'
PS C:\> Test-Json $json_str
True

In this example, a JSON string is stored in the $json_str variable. The Test-Json cmdlet is then executed by passing this variable as input. As the input object is in the JSON format, it returns True. 

## tldr 
 
> Tests whether a string is a valid JSON document.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/test-json>.

- Test if a string from stdin is in JSON format:

`'{{string}}' | Test-Json`

- Test if a string JSON format:

`Test-Json -Json '{{json_to_test}}'`

- Test if a string from stdin matches a specific schema file:

`'{{string}}' | Test-Json -SchemaFile {{path\to\schema_file.json}}`
