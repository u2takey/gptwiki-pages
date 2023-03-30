# unalias 
## chatgpt 
The "unalias" command is used in Unix-like operating systems to remove an alias previously created using the "alias" command. An alias is a shortcut that points to a longer command or sequence of commands. 

The syntax for the "unalias" command is simple: 

```unalias [alias name]```

Where "alias name" is the name of the alias you want to remove. If no alias name is specified, all aliases are removed.

When executed, the "unalias" command will immediately remove the specified alias from the current shell session, and the alias will no longer be accessible using that name. This can be helpful in cleaning up your shell environment, or in disabling aliases that are causing conflicts or errors.

For example, suppose that you had previously created an alias named "ll" that stood for "ls -l", but you no longer want to use this alias. To remove it, you would simply enter:

```unalias ll```

This would remove the "ll" alias from your current shell session, and typing "ll" would no longer produce the same output as "ls -l". 

## tldr 
 
> Remove aliases.
> More information: <https://manned.org/unalias>.

- Remove an alias:

`unalias {{alias_name}}`

- Remove all aliases:

`unalias -a`
