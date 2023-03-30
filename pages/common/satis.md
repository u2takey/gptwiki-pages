# satis 
## chatgpt 
I'm sorry, which specific command are you referring to? "Satis" is not a recognized command on its own. Please provide more context or information. 

## tldr 
 
> The command-line utility for the Satis static Composer repository.
> More information: <https://github.com/composer/satis>.

- Initialize a Satis configuration:

`satis init {{satis.json}}`

- Add a VCS repository to the Satis configuration:

`satis add {{repository_url}}`

- Build the static output from the configuration:

`satis build {{satis.json}} {{path/to/output_directory}}`

- Build the static output by updating only the specified repository:

`satis build --repository-url {{repository_url}} {{satis.json}} {{path/to/output_directory}}`

- Remove useless archive files:

`satis purge {{satis.json}} {{path/to/output_directory}}`
