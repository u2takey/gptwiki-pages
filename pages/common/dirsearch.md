# dirsearch 
## chatgpt 
The command "dirsearch" is a tool used for performing a directory brute-forcing attack on a target website. The tool recursively scans the directory structure of a web server, looking for hidden directories and files that typically contain sensitive information such as configuration files, backup files, administrator interfaces, and more.

The syntax of the command typically looks like this:
dirsearch [OPTIONS] URL

Here, "OPTIONS" represent the various parameters that can be passed to the tool, while "URL" represents the target website's URL. Some of the most commonly used options include:

-recursion-depth: This option is used to set the recursive depth of the tool's search. By default, the tool is set to 2 levels of recursion, but this can be increased or decreased as needed.

-extensions: This option is used to specify file extensions to be included in the search.

-wordlist: This option is used to specify a custom wordlist to be used in the directory brute-forcing attack.

-threads: This option is used to specify the number of threads used for the scan. More threads mean faster scanning but can also lead to server overload, so this option should be used carefully.

Overall, the dirsearch tool is a powerful tool for performing directory brute-forcing attacks on web servers and can help to uncover hidden vulnerabilities and sensitive information that may not be accessible through normal means. 

## tldr 
 
> Web path scanner.
> More information: <https://github.com/maurosoria/dirsearch>.

- Scan a web server for common paths with common extensions:

`dirsearch --url {{url}} --extensions-list`

- Scan a list of web servers for common paths with the `.php` extension:

`dirsearch --url-list {{path/to/url-list.txt}} --extensions {{php}}`

- Scan a web server for user-defined paths with common extensions:

`dirsearch --url {{url}} --extensions-list --wordlist {{path/to/url-paths.txt}}`

- Scan a web server using a cookie:

`dirsearch --url {{url}} --extensions {{php}} --cookie {{cookie}}`

- Scan a web server using the `HEAD` HTTP method:

`dirsearch --url {{url}} --extensions {{php}} --http-method {{HEAD}}`

- Scan a web server, saving the results to a `.json` file:

`dirsearch --url {{url}} --extensions {{php}} --json-report {{path/to/report.json}}`
