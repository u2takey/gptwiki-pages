# linkchecker 
## chatgpt 
Linkchecker is a command-line tool used for checking the validity of links on a website. It checks links for their functionality and status (either active or broken) and generates a report of the status of every link on the website.

To use the linkchecker command, you need to install the tool on your computer. Once installed, you can open the command prompt or terminal and run the linkchecker command followed by the website URL that you want to check like this:

linkchecker <websiteURL>

For example, if you want to check the links on the website example.com, you would enter the following command:

linkchecker https://example.com

Once the command is executed, the tool will start to check all the links on the website and will generate a report that can be viewed in a separate window or saved to a file using the --output option.

Linkchecker has various options that can be used to customize its behavior, including the number of threads to use, the depth of the link search, and the types of links to ignore or include in the check. You can find all the available options in the linkchecker documentation. 

## tldr 
 
> Command-line client to check HTML documents and websites for broken links.
> More information: <https://linkchecker.github.io/linkchecker/>.

- Find broken links on https://example.com/:

`linkchecker {{https://example.com/}}`

- Also check URLs that point to external domains:

`linkchecker --check-extern {{https://example.com/}}`

- Ignore URLs that match a specific regular expression:

`linkchecker --ignore-url {{regular_expression}} {{https://example.com/}}`

- Output results to a CSV file:

`linkchecker --file-output {{csv}}/{{path/to/file}} {{https://example.com/}}`
