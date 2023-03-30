# lwp-request 
## chatgpt 
The lwp-request command is used to send HTTP requests to web servers and fetch the corresponding responses. The lwp-request command is a command-line tool that uses the LWP (Library for WWW in Perl) libraries to make HTTP requests. Here is a detailed explanation of the command:

Usage: lwp-request [options...] [http://]host[:port]/[path]

Options:
 -M http_method   HTTP method (GET, POST, HEAD, PUT, DELETE, etc.)
 -H header        Additional headers to include in HTTP request
 -d data          Data to include in HTTP request (for POST/PUT requests)
 -u username      Username for HTTP Basic authentication
 -p password      Password for HTTP Basic authentication
 -e email         Email address for HTTP Digest authentication
 -r realm         Realm for HTTP Digest authentication
 -c count         Number of times to repeat the request
 -s seconds       Time to sleep between repetitions
 -o filename      Write response to file instead of STDOUT
 -h               Show help and usage information

The lwp-request command uses the standard HTTP methods (GET, POST, HEAD, PUT, DELETE, etc.) to make requests to web servers. It can also include additional headers, data, and authentication information in the HTTP requests.

The host and port parameters specify the target web server, and the path parameter specifies the resource to request from the server. If the path parameter is not specified, the server will return the default resource (usually the index page).

The -c and -s options are used to repeat requests multiple times, with a delay between each request. The -o option is used to write the response to a file instead of displaying it on the command line.

In summary, the lwp-request command is a versatile tool for making HTTP requests and fetching the resulting responses, with support for various HTTP methods, headers, data, and authentication methods. 

## tldr 
 
> Simple command-line HTTP client.
> Built with libwww-perl.
> More information: <https://metacpan.org/pod/lwp-request>.

- Make a simple GET request:

`lwp-request -m GET {{http://example.com/some/path}}`

- Upload a file with a POST request:

`lwp-request -m POST {{http://example.com/some/path}} < {{path/to/file}}`

- Make a request with a custom user agent:

`lwp-request -H 'User-Agent: {{user_agent}} -m {{METHOD}} {{http://example.com/some/path}}`

- Make a request with HTTP authentication:

`lwp-request -C {{username}}:{{password}} -m {{METHOD}} {{http://example.com/some/path}}`

- Make a request and print request headers:

`lwp-request -U -m {{METHOD}} {{http://example.com/some/path}}`

- Make a request and print response headers and status chain:

`lwp-request -E -m {{METHOD}} {{http://example.com/some/path}}`
