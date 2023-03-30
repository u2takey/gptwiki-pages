# curl 
## chatgpt 
`curl` is a command-line tool used to transfer data to or from a server. It sends HTTP requests to the server and displays the response sent back by the server. 

The basic syntax for the `curl` command is as follows:

```
curl [options] [URL]
```

Here, `options` are the various flags or switches that can be used to customize the request and response behavior. `URL` is the server URL to which the HTTP request needs to be sent.

Some commonly used options with `curl` command are:

- `-X`: used to specify the HTTP request method like GET, POST, PUT, DELETE, etc.
- `-d`: used to pass data along with the HTTP request body.
- `-H`: used to specify the custom headers to be sent along with the request.
- `-i`: displays the HTTP response headers as well.
- `-L`: follow any redirect returned by the server.
- `-o`: saves the output to a file.

For example, consider the following command:

```
curl -X POST -d "username=alice&password=secret" https://example.com/login
```

Here, we are sending a POST request with username and password as parameters using the `-d` flag. The `-X` flag specifies the HTTP request method to be used. The server URL is `https://example.com/login`.

The `curl` command is widely used in shell scripts and automation tasks as it provides a quick and easy way to interact with web servers and APIs from the command line. 

## tldr 
 
> Transfers data from or to a server.
> Supports most protocols, including HTTP, FTP, and POP3.
> More information: <https://curl.se>.

- Download the contents of a URL to a file:

`curl {{http://example.com}} --output {{path/to/file}}`

- Download a file, saving the output under the filename indicated by the URL:

`curl --remote-name {{http://example.com/filename}}`

- Download a file, following location redirects, and automatically continuing (resuming) a previous file transfer and return an error on server error:

`curl --fail --remote-name --location --continue-at - {{http://example.com/filename}}`

- Send form-encoded data (POST request of type `application/x-www-form-urlencoded`). Use `--data @file_name` or `--data @'-'` to read from STDIN:

`curl --data {{'name=bob'}} {{http://example.com/form}}`

- Send a request with an extra header, using a custom HTTP method:

`curl --header {{'X-My-Header: 123'}} --request {{PUT}} {{http://example.com}}`

- Send data in JSON format, specifying the appropriate content-type header:

`curl --data {{'{"name":"bob"}'}} --header {{'Content-Type: application/json'}} {{http://example.com/users/1234}}`

- Pass a username and password for server authentication:

`curl --user myusername:mypassword {{http://example.com}}`

- Pass client certificate and key for a resource, skipping certificate validation:

`curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://example.com}}`
