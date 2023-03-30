# django-admin 
## chatgpt 
`django-admin` is a command-line tool used to perform various administrative tasks related to Django, a web framework for building web applications. 

When the `django-admin` command is executed in the terminal, it provides a list of available subcommands that can be used to perform a variety of tasks. These subcommands include:

- `startproject`: creates a new Django project
- `startapp`: creates a new Django application
- `runserver`: starts the development server
- `makemigrations`: creates new database migration files based on changes in the models
- `migrate`: applies pending database migrations
- `createsuperuser`: creates a new superuser for the Django admin site
- `collectstatic`: collects all static files into a single location for deployment
- `test`: runs tests for the Django application

Each subcommand can be followed by additional arguments and options to customize the behavior of the command. For example, `django-admin startproject myproject` will create a new Django project named `myproject`. 

Overall, `django-admin` is a powerful tool that makes it easy to manage and develop Django projects from the command line. 

## tldr 
 
> Django’s utility for administrative tasks.
> More information: <https://docs.djangoproject.com/en/4.1/ref/django-admin/>.

- Create a new Django project:

`django-admin startproject {{project_name}}`

- Create a new app for the current project:

`django-admin startapp {{app_name}}`

- Check the current version of Django:

`django-admin --version`

- Display more information for the given command:

`django-admin help {{command}}`
