# http-prompt 
## chatgpt 
The `http-prompt` command is a user-friendly HTTP client in the form of an interactive shell-like command line tool. It helps in executing HTTP requests, inspecting HTTP responses, and exploring HTTP APIs easily, without the need of leaving the command line interface.

When the `http-prompt` command is executed, the tool starts an interactive shell environment that displays a prompt in the following format: `(base) http://localhost:8000/>`, where the `localhost:8000` is the default base URL of the API. The user can change the base URL by using the `set base_url` command.

The shell prompt is equipped with several built-in commands (also known as `http-prompt commands`) that enable the user to perform various tasks related to networking and HTTP requests. Some of the commonly used commands are GET, POST, PUT, DELETE, PATCH, etc. Each command requires a specific URL to work on, for example, the GET command accepts a URL endpoint as its parameter, and it returns the response data from the server.

The `http-prompt` command also comes with various helpful features, such as auto-completion, syntax highlighting, and customization options. Additionally, it allows the user to save and load their session data, which can be useful for debugging and testing purposes.

Overall, `http-prompt` is a very useful tool for developers and system administrators who perform HTTP-based operations frequently. It simplifies the process of performing HTTP requests and helps in quickly troubleshooting API issues from the command line interface. 

## tldr 
 
> An interactive command-line HTTP client featuring autocomplete and syntax highlighting.
> More information: <https://github.com/httpie/http-prompt>.

- Launch a session targeting the default URL of http://localhost:8000 or the previous session:

`http-prompt`

- Launch a session with a given URL:

`http-prompt {{http://example.com}}`

- Launch a session with some initial options:

`http-prompt {{localhost:8000/api}} --auth {{username:password}}`
