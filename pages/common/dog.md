# dog 
## chatgpt 
As an AI language model, I want to clarify that 'dog' is not a valid command in most operating systems, including Windows, Mac OS, or Linux. However, 'dog' is a common Unix/Linux command that helps to display the contents of a file on the terminal. 

The 'dog' command is actually an alias for the Linux command 'cat' (concatenate), and it stands for "DO the Grep." The 'grep' command is another common Unix/Linux command that is used to search for a particular string of text within a file.

Using the 'dog' command, you can display the contents of a single file or multiple files in the terminal. For instance, the syntax for the 'dog' command is:

```
dog <filename>
```

Here, you can replace `<filename>` with the name of the file that you want to display. If you want to print multiple files, you can specify their names separated by spaces like:

```
dog file1.txt file2.txt
```

The 'dog' command displays the contents of the file(s) on the terminal in a similar way as the 'cat' command. The difference between these two commands is that 'dog' applies syntax highlighting to the output and provides a more user-friendly and interactive display. 

## tldr 
 
> DNS lookup utility.
> It has colorful output, supports DNS-over-TLS and DNS-over-HTTPS protocols, and can emit JSON.
> More information: <https://dns.lookup.dog>.

- Lookup the IP(s) associated with a hostname (A records):

`dog {{example.com}}`

- Query the MX records type associated with a given domain name:

`dog {{example.com}} MX`

- Specify a specific DNS server to query (e.g. Cloudflare):

`dog {{example.com}} MX @{{1.1.1.1}}`

- Query over TCP rather than UDP:

`dog {{example.com}} MX @{{1.1.1.1}} --tcp`

- Query the MX records type associated with a given domain name over TCP using explicit arguments:

`dog --query {{example.com}} --type MX --nameserver {{1.1.1.1}} --tcp`

- Lookup the IP(s) associated with a hostname (A records) using DNS over HTTPS (DoH):

`dog {{example.com}} --https @{{https://cloudflare-dns.com/dns-query}}`
