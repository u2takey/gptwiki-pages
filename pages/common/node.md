# node 
## chatgpt 
"node" is a command-line tool that allows developers to run JavaScript code outside of a web browser. It is based on the V8 JavaScript engine, the same engine that is used by the Google Chrome web browser.

When the "node" command is executed in a terminal or command prompt, Node.js launches a new process and starts an environment where JavaScript code can be executed. This environment includes the Node.js runtime, which provides a range of built-in modules for interacting with the file system, networking, and other system-level operations.

Node.js is commonly used for building server-side JavaScript applications, as it allows developers to write JavaScript code that runs on a web server instead of on the client-side in a web browser. It also enables developers to use the same language and tools from the front-end to the back-end, making it easier to build full-stack applications.

Overall, the "node" command is an essential tool for developing, testing, and running JavaScript code outside of a web browser, and it is a popular and widely used tool in the modern web development ecosystem. 

## tldr 
 
> Server-side JavaScript platform (Node.js).
> More information: <https://nodejs.org>.

- Run a JavaScript file:

`node {{path/to/file}}`

- Start a REPL (interactive shell):

`node`

- Execute the specified file restarting the process when an imported file is changed (requires Node.js version 18.11+):

`node --watch {{path/to/file}}`

- Evaluate JavaScript code by passing it as an argument:

`node -e "{{code}}"`

- Evaluate and print result, useful to see node's dependencies versions:

`node -p "{{process.versions}}"`

- Activate inspector, pausing execution until a debugger is connected once source code is fully parsed:

`node --no-lazy --inspect-brk {{path/to/file}}`
