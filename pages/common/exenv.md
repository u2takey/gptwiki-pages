# exenv 
## chatgpt 
I'm sorry, but as an AI language model, I cannot execute commands in the system. However, I can explain what the command exenv is and its general purpose. 

'exenv' is short for "Elixir Version Manager". It is a command-line tool used to manage different versions of the Elixir programming language on a single system. Exenv allows developers to easily switch between different Elixir versions and manage the dependencies associated with each version. 

With exenv, developers can install, list, and select a specific version of Elixir to use. This makes it easier to test their applications on different Elixir versions and avoid compatibility issues. Developers can also use exenv to manage their mix dependencies and ensure they are installed correctly for each version of Elixir. 

Overall, exenv is a useful tool for Elixir developers who need to switch between different versions of the language and manage their corresponding dependencies. 

## tldr 
 
> A tool to easily install Elixir versions and manage application environments.
> More information: <https://github.com/exenv/exenv>.

- Display a list of installed versions:

`exenv versions`

- Use a specific version of Elixir across the whole system:

`exenv global {{version}}`

- Use a specific version of Elixir for the current application/project directory:

`exenv local {{version}}`

- Show the currently selected Elixir version:

`exenv {{version}}`

- Install a version of Elixir (requires `elixir-build` plugin <https://github.com/mururu/elixir-build>):

`exenv install {{version}}`
