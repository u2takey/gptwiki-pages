# httpie 
## chatgpt 
HTTPie is a command-line tool for making HTTP requests, similar to cURL. HTTPie makes it easy to interact with web services and APIs, providing a simple and intuitive interface for sending HTTP requests and receiving responses.

To use HTTPie, you can simply enter the “http” command followed by the URL you want to send a request to, like this:

```
http https://example.com
```

This will send a GET request to https://example.com and display the response in your console.

HTTPie offers a wide range of options and settings for customizing your requests. For example, you can specify the data or parameters you want to send with your request using the --data or --json options, like this:

```
http POST https://example.com/login username=johndoe password=secret123
```

You can also specify custom headers, cookies, or timeouts using the --headers, --cookies, or --timeout options, respectively.

HTTPie also provides built-in support for many common authentication schemes, including basic auth and OAuth. You can specify the authentication details using the --auth option, like this:

```
http --auth user:password https://example.com
```

Overall, HTTPie provides a powerful and flexible tool for interacting with web services and APIs using the command line. Its intuitive syntax and extensive feature set make it a popular choice for developers and sysadmins alike. 

## tldr 
 
> A user friendly command-line HTTP tool.
> More information: <https://github.com/httpie/httpie>.

- Send a GET request (default method with no request data):

`http {{https://example.com}}`

- Send a POST request (default method with request data):

`http {{https://example.com}} {{hello=World}}`

- Send a POST request with redirected input:

`http {{https://example.com}} < {{file.json}}`

- Send a PUT request with a given JSON body:

`http PUT {{https://example.com/todos/7}} {{hello=world}}`

- Send a DELETE request with a given request header:

`http DELETE {{https://example.com/todos/7}} {{API-Key:foo}}`

- Show the whole HTTP exchange (both request and response):

`http -v {{https://example.com}}`

- Download a file:

`http --download {{https://example.com}}`

- Follow redirects and show intermediary requests and responses:

`http --follow --all {{https://example.com}}`
