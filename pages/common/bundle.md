# bundle 
## chatgpt 
The `bundle` command is a command-line tool primarily used in Ruby on Rails applications. It's part of the `Bundler` gem, which provides a way to manage dependencies for Ruby projects.

When you run the `bundle` command in your project directory, it reads the `Gemfile` file and downloads or installs the required gems or libraries in your project. A `Gemfile` is a file that lists all the gems you need for your project to run smoothly.

Here's what happens when you run the `bundle` command:

1. Bundler checks for a `Gemfile.lock` file. This file contains a list of exact gem versions used in a previous run, so it can skip dependency resolution and use the same versions of each gem.

2. Bundler reads your project's `Gemfile`, which specifies the dependencies required by your application.

3. Bundler checks if the requested gems are already installed on your system or in a shared location.

4. If any gems are not installed, Bundler downloads them from the internet and installs them on your system.

5. When everything has been installed successfully, Bundler updates the `Gemfile.lock` file with the exact versions of each gem that it installed.

In summary, the `bundle` command installs and manages a project's dependencies, ensuring that everyone working on the project is using the same version of each gem or library. It's a vital tool in any Ruby on Rails development environment. 

## tldr 
 
> Dependency manager for the Ruby programming language.
> More information: <https://bundler.io/man/bundle.1.html>.

- Install all gems defined in the `Gemfile` expected in the working directory:

`bundle install`

- Execute a command in the context of the current bundle:

`bundle exec {{command}} {{arguments}}`

- Update all gems by the rules defined in the `Gemfile` and regenerate `Gemfile.lock`:

`bundle update`

- Update one or more specific gem(s) defined in the `Gemfile`:

`bundle update {{gem_name}} {{gem_name}}`

- Update one or more specific gems(s) defined in the `Gemfile` but only to the next patch version:

`bundle update --patch {{gem_name}} {{gem_name}}`

- Update all gems within the given group in the `Gemfile`:

`bundle update --group {{development}}`

- List installed gems in the `Gemfile` with newer versions available:

`bundle outdated`

- Create a new gem skeleton:

`bundle gem {{gem_name}}`
