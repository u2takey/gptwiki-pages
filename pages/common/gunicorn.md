# gunicorn 
## chatgpt 
Gunicorn or 'Green Unicorn' is a lightweight Python HTTP server aimed to help web developers to build scalable applications. It is specifically designed to support the Python WSGI (Web Server Gateway Interface) specification that helps web frameworks, such as Django, Flask and Pyramid, to interface with web servers by providing a standard interface between the web applications and the servers, allowing them to communicate with each other.

Gunicorn is a command-line executable program that runs a WSGI application for multiple workers, each handling a single request at a time. It is built on the same asynchronous worker model as Nginx or Apache, which enables it to handle a large number of concurrent connections and perform well under heavy workloads.

Here are some command-line options that can be used with Gunicorn:

`-b` or `--bind`: specifies the IP address and port number on which the server should bind.

`-w` or `--workers`: specifies the number of worker processes to handle incoming requests.

`-t` or `--timeout`: specifies the number of seconds a worker can take to process a request before being terminated.

`-k` or `--worker-class`: specifies the worker class to use.

`-D` or `--daemon`: runs Gunicorn in the background as a daemon process.

For example, to start a Gunicorn server running a Flask application, we might use the following command:

```
gunicorn --workers 4 --bind 0.0.0.0:8000 myapp:app
```

This command will start four worker processes and bind them to port 8000 of the server. `myapp` refers to the name of the Python module containing the Flask application, and `app` is the name of the Flask instance inside that module.

Overall, Gunicorn is a powerful and lightweight server that provides an easy-to-use command-line interface for running Python web applications, making it a popular choice for developers who want a scalable and high-performance web server. 

## tldr 
 
> Python WSGI HTTP Server.
> More information: <https://gunicorn.org/>.

- Run Python web app:

`gunicorn {{import.path:app_object}}`

- Listen on port 8080 on localhost:

`gunicorn --bind {{localhost}}:{{8080}} {{import.path:app_object}}`

- Turn on live reload:

`gunicorn --reload {{import.path:app_object}}`

- Use 4 worker processes for handling requests:

`gunicorn --workers {{4}} {{import.path:app_object}}`

- Use 4 worker threads for handling requests:

`gunicorn --threads {{4}} {{import.path:app_object}}`

- Run app over HTTPS:

`gunicorn --certfile {{cert.pem}} --keyfile {{key.pem}} {{import.path:app_object}}`
