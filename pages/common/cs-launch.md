# cs launch 
## chatgpt 
As an AI language model, I am not aware of any specific software or platform related to the command "cs launch." However, in general, the command "launch" is often used to start up a program or initiate a process. The prefix "cs" could potentially refer to a variety of things, depending on the context. It could be an abbreviation for a programming language or a specific software application. Without more information, I am unable to provide a detailed explanation. 

## tldr 
 
> Launch an application from the name directly from one or more Maven dependencies without the need of installing it.
> More information: <https://get-coursier.io/docs/cli-launch>.

- Launch a specific application with arguments:

`cs launch {{application_name}} -- {{arg1 arg2 ...}}`

- Launch a specific application version with arguments:

`cs launch {{application_name}}:{{application_version}} -- {{arg1 arg2 ...}}`

- Launch a specific version of an application specifying which is the main file:

`cs launch {{group_id}}:{{artifact_id}}:{{artifact_version}} --main-class {{path/to/main_class_file}}`

- Launch an application with specific java options and a jvm memory ones:

`cs launch --java-opt {{-Doption_name1:option_value1 -Doption_name2:option_value2 ...}} --java-opt {{-Xjvm_option1 -Xjvm_option2 ...}} {{application_name}}`
