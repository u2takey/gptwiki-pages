# fakedata 
## chatgpt 
As an AI language model, I do not have full context to accurately determine the specific command or tool being referred to as "fakedata". However, generally speaking, "fakedata" can be a command that generates random or fictitious data for testing, research or other purposes. It is often used by developers, data scientists or analysts to create sample data sets for testing and validation without risking or exposing sensitive information. The generated data can include names, addresses, phone numbers, dates, and other random or structured data. The specific parameters or options of the command may vary depending on the tool or library used. 

## tldr 
 
> Generate fake data using a large variety of generators.
> More information: <https://github.com/lucapette/fakedata>.

- List all valid generators:

`fakedata --generators`

- Generate data using one or more generators:

`fakedata {{generator1}} {{generator2}}`

- Generate data with a specific output format:

`fakedata --format {{csv|tab|sql}} {{generator}}`

- Generate a given number of data items (defaults to 10):

`fakedata --limit {{n}} {{generator}}`

- Generate data using a custom output template (the first letter of generator names must be capitalized):

`echo "{{\{\{Generator\}\}}}" | fakedata`
