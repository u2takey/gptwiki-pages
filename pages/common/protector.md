# protector 
## chatgpt 
As an AI language model, I cannot provide specific details about a command named "protector" as the functionality may vary based on the system or software it is associated with. 

However, generally speaking, a "protector" can refer to a program or tool that is designed to provide security and protection to a system, file, or program. It can be a hardware device, a software program, or a combination of both, depending on the situation.

In some cases, "protector" refers to a command that is used to start or stop a certain process or application on a computer. For instance, a command like "protector start" may be used to initiate a protective measure, while "protector stop" may be used to deactivate it.

Overall, the term "protector" is used in different contexts, and the command related to it will vary depending on the specific use case. 

## tldr 
 
> Protect or unprotect branches on GitHub repositories.
> More information: <https://github.com/jcgay/protector>.

- Protect branches of a GitHub repository (create branch protection rules):

`protector {{branches_regex}} -repos {{organization/repository}}`

- Use the dry run to see what would be protected (can also be used for freeing):

`protector -dry-run {{branches_regex}} -repos {{organization/repository}}`

- Free branches of a GitHub repository (delete branch protection rules):

`protector -free {{branches_regex}} -repos {{organization/repository}}`
