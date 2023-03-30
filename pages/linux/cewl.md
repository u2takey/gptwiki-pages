# cewl 
## chatgpt 
cewl is a command-line tool that stands for "Custom Word List generator." It is a tool used for creating custom wordlists by spidering a target's website and gathering data such as email addresses, usernames, and other relevant information. 

The cewl command is used to call the cewl tool and execute its functionalities. The basic syntax of the command is as follows:

cewl [URL] [OPTIONS]

Where:
- [URL] represents the target website URL.
- [OPTIONS]: this refers to the different options available with the cewl command. Here, you can add arguments to the command to specify output or limit the scope of the generated wordlist.

Some examples of options include:
- -w: This allows you to specify the output file name.
- -d: This option lets you specify the depth of the spidering process, i.e., how many layers deep to crawl.
- -m: This option allows you to specify a minimum word length for words to be included in the generated wordlist.
- -e: This specifies the file extension to include in the wordlist.

For example, to generate a wordlist of the site example.com, the command would be:

cewl example.com

And to save the output to a particular file, you can add the -w option followed by the desired filename:

cewl example.com -w output.txt

Overall, the cewl command is a useful tool for performing reconnaissance and generating custom wordlists that can be used for password cracking or other security testing purposes. 

## tldr 
 
> URL spidering tool for making a cracking wordlist from web content.
> More information: <https://digi.ninja/projects/cewl.php>.

- Create a wordlist file from the given URL up to 2 links depth:

`cewl --depth {{2}} --write {{path/to/wordlist.txt}} {{url}}`

- Output an alphanumeric wordlist from the given URL with words of minimum 5 characters:

`cewl --with-numbers --min_word_length {{5}} {{url}}`

- Output a wordlist from the given URL in debug mode including email addresses:

`cewl --debug --email {{url}}`

- Output a wordlist from the given URL using HTTP Basic or Digest authentication:

`cewl --auth_type {{basic|digest}} --auth_user {{username}} --auth_pass {{password}} {{url}}`

- Output a wordlist from the given URL through a proxy:

`cewl --proxy_host {{host}} --proxy_port {{port}} {{url}}`
