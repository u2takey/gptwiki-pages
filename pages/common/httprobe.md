# httprobe 
## chatgpt 
The command "httprobe" is a tool used in penetration testing and web development to test whether a list of HTTP or HTTPS URLs are live and working correctly. It's also useful for quickly scanning a large number of web pages to determine which are active and which are not.

The "httprobe" tool sends an HTTP/HTTPS request to each URL in the list and waits for a response. If a response is received, it confirms that the URL is live and working correctly. The tool is particularly useful for identifying active web pages that might be hidden deep within a large website with many pages. 

To use "httprobe," you will need to provide it with a list of URLs to check. The URLs can be provided as either a list on the command line or by reading from a text file using input redirection. For example:

```
httbprobe example.com https://google.com http://facebook.com
```

In this example, httprobe is checking three URLs - example.com, google.com, and facebook.com. 

The output of the command will be a list of URLs that have responded with a 200 status code. It can also display additional information, such as the response time and size, by adding the "-v" flag. 

```
http://example.com
https://google.com
http://facebook.com
```

Overall, "httprobe" is a convenient tool for quickly checking the availability and status of a list of URLs, saving you time when testing or developing web applications. 

## tldr 
 
> Take a list of domains and probe for working HTTP and HTTPS servers.
> More information: <https://github.com/tomnomnom/httprobe>.

- Probe a list of domains from a text file:

`cat {{input_file}} | httprobe`

- Only check for HTTP if HTTPS is not working:

`cat {{input_file}} | httprobe --prefer-https`

- Probe additional ports with a given protocol:

`cat {{input_file}} | httprobe -p {{https:2222}}`

- Output all available options:

`httprobe --help`
