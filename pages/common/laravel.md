# laravel 
## chatgpt 
Laravel is a PHP framework that simplifies web development. It provides useful tools and features for building applications quickly and effectively. The command "laravel" is used to create a new Laravel project. Here are the steps involved in creating a new Laravel project using the "laravel" command:

1. Open the terminal (command prompt) and navigate to the directory where you want to create the project.

2. Type the following command and hit "Enter":
```
laravel new project-name
```

3. Laravel will now download and install all the necessary dependencies and create a new project with the name you provided (replace "project-name" with the actual name you want to use).

4. Once the project is successfully created, navigate to the project directory using the following command:
```
cd project-name
```

Now you are ready to start building your Laravel application. The "laravel" command is also used for other tasks such as performing database migrations, running tests, and generating code scaffolding. To learn more about Laravel and its capabilities, visit the official documentation website. 

## tldr 
 
> A command-line installer for the Laravel framework.
> More information: <https://laravel.com>.

- Create a new Laravel application:

`laravel new {{name}}`

- Use the latest development release:

`laravel new {{name}} --dev`

- Overwrite if the directory already exists:

`laravel new {{name}} --force`

- Install the Laravel Jetstream scaffolding:

`laravel new {{name}} --jet`

- Install the Laravel Jetstream scaffolding with a specific stack:

`laravel new {{name}} --jet --stack {{livewire|inertia}}`

- Install the Laravel Jetstream scaffolding with support for teams:

`laravel new {{name}} --jet --teams`

- List the available installer commands:

`laravel list`
