# raw 
## chatgpt 
As an AI language model, I cannot provide a specific answer to the question without more context. However, the term "raw" is often used in computing to refer to unprocessed or unformatted data. In the context of a command, "raw" may refer to a file or data type that needs to be processed further in order to be usable. It could also be a flag that is added to a command to indicate that the output should be unprocessed and not formatted. More information is needed to provide a more detailed answer. 

## tldr 
 
> Bind a Unix raw character device.
> More information: <https://manned.org/raw.8>.

- Bind a raw character device to a block device:

`raw /dev/raw/raw{{1}} {{/dev/block_device}}`

- Query an existing binding instead of setting a new one:

`raw /dev/raw/raw{{1}}`

- Query all bound raw devices:

`raw -qa`
