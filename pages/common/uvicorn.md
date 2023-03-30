# uvicorn 
## chatgpt 
Uvicorn is a Python ASGI (Asynchronous Server Gateway Interface) server that is used to run Python web applications. It stands for "Unicorn" which is a mythical horse-like creature with a single horn on its forehead. 

The command "uvicorn" is used to start the Uvicorn server and run the application. It takes a few arguments like:

1. The path to the Python web application module.
2. The host IP address and port number where the server listens for incoming connections. By default, it listens on localhost on port 8000.
3. The number of workers that should be used for handling incoming requests.

Some examples of the uvicorn command are:

- uvicorn myapp:app (Runs the "app" object defined in the "myapp" module. It listens on the default localhost:8000)
- uvicorn myapp:app --host 0.0.0.0 --port 8080 (Runs the "app" object defined in the "myapp" module. It listens on all network interfaces on port 8080)
- uvicorn myapp:app --workers 4 (Runs the "app" object defined in the "myapp" module with 4 worker processes)

Overall, the "uvicorn" command is a handy utility to run Python web applications using the ASGI protocol in a production environment. 

## tldr 
 
> Python ASGI HTTP Server, for asynchronous projects.
> More information: <https://www.uvicorn.org/>.

- Run Python web app:

`uvicorn {{import.path:app_object}}`

- Listen on port 8080 on localhost:

`uvicorn --host {{localhost}} --port {{8080}} {{import.path:app_object}}`

- Turn on live reload:

`uvicorn --reload {{import.path:app_object}}`

- Use 4 worker processes for handling requests:

`uvicorn --workers {{4}} {{import.path:app_object}}`

- Run app over HTTPS:

`uvicorn --ssl-certfile {{cert.pem}} --ssl-keyfile {{key.pem}} {{import.path:app_object}}`
