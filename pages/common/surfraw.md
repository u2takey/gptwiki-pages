# surfraw 
## chatgpt 
Surfraw is a command-line tool that allows users to search and navigate the internet using a variety of text-based interfaces. It stands for "Shell Users' Revolutionary Front Rage Against the Web" and is designed to offer users a fast and efficient way to search the web without having to deal with the clutter of graphical user interfaces.

The surfraw command launches the Surfraw shell and allows users to enter search queries and navigate the web using a variety of different search engines and services. Additionally, Surfraw provides a number of helpful features, including command history, tab completion, and the ability to specify different search engines and services by using a variety of different command-line arguments.

For example, using the command "surfraw google hello world" would launch the Surfraw shell and use the Google search engine to search for information about the phrase "hello world." Similarly, using the command "surfraw wikipedia surfraw" would search the Wikipedia website for information about the Surfraw tool.

Overall, the surfraw command is a powerful and versatile tool for quickly searching and navigating the internet from the command line. Its simplicity and efficiency make it an excellent choice for users who prefer text-based interfaces and want to save time and reduce distractions while browsing the web. 

## tldr 
 
> CLI to query a variety of web search engines.
> Consists of a collection of elvi, each of which knows how to search a specific website.
> More information: <http://surfraw.org>.

- Display the list of supported website search scripts (elvi):

`surfraw -elvi`

- Open the elvi's results page for a specific search in the browser:

`surfraw {{elvi}} "{{search_terms}}"`

- Display an elvi description and its specific options:

`surfraw {{elvi}} -local-help`

- Search using an elvi with specific options and open the results page in the browser:

`surfraw {{elvi}} {{elvi_options}} "{{search_terms}}"`

- Display the URL to the elvi's results page for a specific search:

`surfraw -print {{elvi}} "{{search_terms}}"`

- Search using the alias:

`sr {{elvi}} "{{search_terms}}"`
