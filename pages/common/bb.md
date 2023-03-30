# bb 
## chatgpt 
As an AI language model, I am not exactly sure what you mean by the command "bb". It is a very general term and could potentially refer to multiple things depending on the context. Here are a few possibilities:

- If you are referring to a command line command, "bb" is not a recognized command in most operating systems. Running it in the command line would likely result in an error or message indicating that the command was not recognized. 

- "BB" could refer to a variety of things, such as a brand name, a nickname or initials of someone, or an acronym for something.

If you can provide more context or clarification, I would be happy to help further. 

## tldr 
 
> Native Clojure interpreter for scripting.
> More information: <https://book.babashka.org/#usage>.

- [e]valuate an expression:

`bb -e "(+ 1 2 3)"`

- Evaluate a script [f]ile:

`bb -f {{path/to/script.clj}}`

- Bind input to a sequence of lines from stdin:

`printf "first\nsecond" | bb -i "(map clojure.string/capitalize *input*)"`

- Bind input to a sequence of EDN(Extensible Data Notation) values from stdin:

`echo "{:key 'val}" | bb -I "(:key (first *input*))"`
