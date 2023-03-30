# prqlc 
## chatgpt 
Sorry, as an AI language model, I couldn't find any meaningful information related to the "prqlc" command. It might be a custom or proprietary command specific to a particular system or software. Can you please provide more context or information about where you found this command or in which context you want to use it? I would be happy to help you if you could provide me with more details. 

## tldr 
 
> PRQL compiler.
> PRQL is a modern language for transforming data - a simple, powerful, pipelined SQL replacement.
> More information: <https://prql-lang.org>.

- Run the compiler interactively:

`prqlc compile`

- Compile a specific `.prql` file to stdout:

`prqlc compile {{path/to/file.prql}}`

- Compile a `.prql` file to a `.sql` file:

`prqlc compile {{path/to/source.prql}} {{path/to/target.sql}}`

- Compile a query:

`echo "{{from employees | filter has_dog | select salary}}" | prqlc compile`

- Watch a directory and compile on file modification:

`prqlc watch {{path/to/directory}}`
