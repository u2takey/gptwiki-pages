# gobuster 
## chatgpt 
Gobuster is a tool used for brute forcing web-based directories and DNS subdomains. It is a command-line tool that can be used for penetration testing and finding hidden content on a website.

The basic syntax of the command to use gobuster is as follows:

gobuster [OPTIONS] WORDLIST URL

Here, the OPTIONS are the various options you can use with the command. Some of the most commonly used ones are:

  -u : the URL you want to check for hidden content
  -w : the path to the wordlist file that contains the words to be used in the brute force attack
  -s : the status codes you want to see returned when the content is found

The WORDLIST is the path to the wordlist file that contains the words to be used in the brute force attack. This file can be created separately or the user can use pre-built wordlists that are available online.

Finally, the URL is the target URL that you want to check for hidden content.

Once the command is executed, gobuster will use the words in the wordlist file to systematically check for hidden content on the target URL. The tool will return any content that it is able to find by following the paths specified in the wordlist file. This can include sensitive directories or files that are hidden from view on the website.

It is important to note that gobuster is a powerful tool and should only be used for legitimate purposes like website testing or penetration testing on sites you own or have permission to test. Unauthorized use of this tool is illegal and can lead to severe consequences. 

## tldr 
 
> Brute-forces hidden paths on web servers and more.
> More information: <https://github.com/OJ/gobuster>.

- Discover directories and files that match in the wordlist:

`gobuster dir --url {{https://example.com/}} --wordlist {{path/to/file}}`

- Discover subdomains:

`gobuster dns --domain {{example.com}} --wordlist {{path/to/file}}`

- Discover Amazon S3 buckets:

`gobuster s3 --wordlist {{path/to/file}}`

- Discover other virtual hosts on the server:

`gobuster vhost --url {{https://example.com/}} --wordlist {{path/to/file}}`

- Fuzz the value of a parameter:

`gobuster fuzz --url {{https://example.com/?parameter=FUZZ}} --wordlist {{path/to/file}}`

- Fuzz the name of a parameter:

`gobuster fuzz --url {{https://example.com/?FUZZ=value}} --wordlist {{path/to/file}}`
