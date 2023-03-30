# http 
## chatgpt 
The command "http" is not a specific command with a standard use or syntax in most operating systems or programming languages. However, it could refer to one of the following:

- The HTTP protocol, which is the primary protocol used for communication between web servers and web clients (such as web browsers). This protocol defines the syntax and structure of requests and responses that are sent over the internet. Using this protocol, a web client can request information from a web server or send information to it, such as submitting a form or uploading a file.

- A command line utility or tool that can send HTTP requests to a web server and display the response. Such tools might include `wget`, `curl`, or `httpie`, among others. These tools typically allow users to specify the specific HTTP request method (such as GET, POST, PUT, etc.), the URL of the server, any query or payload data to be sent with the request, and any headers or other metadata to be included in the request.

- A shorthand or abbreviation that might be used in scripts or programming contexts to refer to the HTTP protocol or an HTTP request/response cycle. For example, someone might refer to "sending an http request" as a way of saying "sending an HTTP request using some tool or library".

Without more context or information about how the command is being used, it is unclear what specific syntax or functionality might be associated with the "http" command, or what operating system or language it might be used in. 

## tldr 
 
> HTTPie: HTTP client, aims to be easier to use than cURL.
> More information: <https://httpie.org>.

- Download a URL to a file:

`http --download {{example.org}}`

- Send form-encoded data:

`http --form {{example.org}} {{name='bob'}} {{profile_picture@'bob.png'}}`

- Send JSON object:

`http {{example.org}} {{name='bob'}}`

- Specify an HTTP method:

`http {{HEAD}} {{example.org}}`

- Include an extra header:

`http {{example.org}} {{X-MyHeader:123}}`

- Pass a username and password for server authentication:

`http --auth {{username:password}} {{example.org}}`

- Specify raw request body via `stdin`:

`cat {{data.txt}} | http PUT {{example.org}}`
