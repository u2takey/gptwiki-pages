# ipaggmanip 
## chatgpt 
I'm sorry, but there is no recognized command "ipaggmanip". Can you please provide more information or context about the command? 

## tldr 
 
> Manipulate aggregate statistics produced by `ipaggcreate`.
> More information: <https://manned.org/ipaggmanip>.

- Combine labels equal in their high-order bits:

`ipaggmanip --prefix {{16}} {{path/to/file}}`

- Remove labels with a count smaller than a given number of bytes and output a random sample of such labels:

`ipaggmanip --cut-smaller {{100}} --cull-labels {{5}} {{path/to/file}}`

- Replace each label's count with 1 if it is non-zero:

`ipaggmanip --posterize {{path/to/file}}`
