# flask 
## chatgpt 
Flask is a Python web framework. It is a command used to initiate a new Flask application or to start an existing Flask application in development mode. When the "flask" command is executed, it searches for the "app.py" file in the current directory or the directory specified in the FLASK_APP environment variable. 

If the "app.py" file is found, it runs the Flask application and serves it on a localhost. By default, Flask runs on port 5000, but this can be changed by setting the FLASK_RUN_PORT environment variable. 

The Flask application can then be accessed by opening a web browser and navigating to http://localhost:5000 or the port number specified in the FLASK_RUN_PORT environment variable.

In addition to starting the Flask application, the "flask" command can also be used to perform other tasks such as running tests, creating a new Flask project, or initializing a database. These tasks are carried out by specifying additional parameters after the "flask" command. For example, "flask initdb" can be used to initialize a database for the Flask application. 

## tldr 
 
> A general utility script for Flask applications. Loads the application defined in the `FLASK_APP` environment variable.
> More information: <https://flask.palletsprojects.com/en/1.1.x/cli/>.

- Run a development server:

`flask run`

- Show the routes for the app:

`flask routes`

- Run a Python interactive shell in the app's context:

`flask shell`
