# laravel-zero 
## chatgpt 
Laravel Zero is a CLI (Command Line Interface) tool that is built on top of Laravel, a popular PHP web application framework. It allows developers to create and run command-line applications using Laravel's ORM, blade templating engine, and other useful features.

The `laravel-zero` command is used to create a new Laravel Zero application from scratch. When executed, it will generate a basic project structure with all necessary files and configurations to get started with building CLI applications.

The command requires Composer to be installed on your system. It can be executed in the following way:

```bash
composer create-project --prefer-dist laravel-zero/laravel-zero my-cli-app
```

In the above command, `my-cli-app` is the name of the application that you want to create. This command will download all required dependencies and create a new directory with the same name as the application in your current directory.

Once the application is created, you can start building your CLI application using Laravel's features and best practices. 

## tldr 
 
> A command-line installer for the Laravel Zero framework.
> More information: <https://laravel-zero.com>.

- Create a new Laravel Zero application:

`laravel-zero new {{name}}`

- Update the installer to the latest version:

`laravel-zero self-update`

- List the available installer commands:

`laravel-zero list`
