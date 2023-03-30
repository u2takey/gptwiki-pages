# monop 
## chatgpt 
As an AI language model, I do not have the authority to execute commands on a physical machine. However, I can provide an explanation of the command "monop" as follows:

Monop is a command-line utility that allows you to play a game of Monopoly on your Linux terminal. It is an open-source alternative to the commercial Monopoly game. It simulates a virtual board game, and the players can roll dice, buy properties, pay rent, and collect money. The game features computer-controlled opponents, customizable rules, and support for multiple languages.

To install monop, you can use the package manager of your Linux distribution (e.g., apt, yum, pacman) and run the command: 

```
sudo apt-get install monop
```

Once installed, you can run the game by typing the command "monop" in your terminal console. You will then be prompted to enter the number of players (including yourself), the names of the players, and the starting money amount.

Monop has a simple and intuitive interface with a text-based graphics display, which allows you to navigate through the game and keep track of your progress. The game is played using the keyboard arrow keys to move and make choices.

Overall, monop is an entertaining command-line game that can provide hours of fun for Linux users. 

## tldr 
 
> Finds and displays signatures of Types and methods inside .NET assemblies.
> More information: <https://manned.org/monop>.

- Show the structure of a Type built-in of the .NET Framework:

`monop {{System.String}}`

- List the types in an assembly:

`monop -r:{{path/to/assembly.exe}}`

- Show the structure of a Type in a specific assembly:

`monop -r:{{path/to/assembly.dll}} {{Namespace.Path.To.Type}}`

- Only show members defined in the specified Type:

`monop -r:{{path/to/assembly.dll}} --only-declared {{Namespace.Path.To.Type}}`

- Show private members:

`monop -r:{{path/to/assembly.dll}} --private {{Namespace.Path.To.Type}}`

- Hide obsolete members:

`monop -r:{{path/to/assembly.dll}} --filter-obsolete {{Namespace.Path.To.Type}}`

- List the other assemblies that a specified assembly references:

`monop -r:{{path/to/assembly.dll}} --refs`
