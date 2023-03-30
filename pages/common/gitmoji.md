# gitmoji 
## chatgpt 
As an AI language model, I don't have access to the Gitmoji command. However, I can provide you some information on Gitmojis.

Gitmojis are used to represent the specific type of changes made in the Git commit messages. It is a way to write the description of the commit messages in a concise and understandable way. In simple words, Gitmojis are a set of emoticons or icons used to communicate the intention of the Git commit message.

For instance, if you have changed the code to fix a bug, you can use the bug emoji, or if you have added a new feature, you can use the feature emoji.

The Gitmoji command is a tool used to simplify the process of writing Git commit messages by providing a list of Gitmojis that you can choose from. It ensures that the commit message is consistent, descriptive, and easy to understand.

To use Gitmoji, you need to first install it on your system by following the instructions mentioned in the Gitmoji documentation. Once installed, you can use Gitmoji by typing `gitmoji` in the terminal or command prompt, and then selecting the appropriate Gitmoji from the list.

Once you have selected the Gitmoji, you can write the rest of your commit message according to your project's Git commit message guidelines. Additionally, you can also add supplementary information, like the issue number, the author of the commit, etc. to make the commit message more useful. 

## tldr 
 
> An interactive command-line tool for using emojis on commits.
> More information: <https://github.com/carloscuesta/gitmoji-cli>.

- Start the commit wizard:

`gitmoji --commit`

- Initialize the git hook (so `gitmoji` will be run every time `git commit` is run):

`gitmoji --init`

- Remove the git hook:

`gitmoji --remove`

- List all available emojis and their descriptions:

`gitmoji --list`

- Search emoji list for a list of keywords:

`gitmoji --search {{keyword1}} {{keyword2}}`

- Update cached list of emojis from main repository:

`gitmoji --update`

- Configure global preferences:

`gitmoji --config`
