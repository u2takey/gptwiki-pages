# hashcat 
## chatgpt 
Hashcat is a command-line tool used for cracking passwords and hashes. It can be used on Linux, Windows, and macOS operating systems.

The command begins with the name of the tool, hashcat, followed by various options and arguments. Here are some examples of the options and arguments you can use:

- *-m*: specifies the hash type that you want to crack. For example, 0 for MD5, 100 for SHA1, 500 for SHA-256, etc.
- *-a*: specifies the attack mode that you want to use. For example, 0 for straight/dictionary attack, 3 for mask attack, etc.
- *-w*: specifies the workload profile that you want to use. For example, 1 for low, 2 for medium, 3 for high, etc.
- *-o*: specifies the output file where the cracked hashes will be stored.
- *-r*: specifies the rule file that you want to use for modifying the wordlist. Rules can be used to add prefixes/suffixes, modify case, reverse words, etc.
- *-1*: specifies the character set for the first position in a mask attack. For example, ?l for lowercase letters, ?u for uppercase letters, ?d for digits, etc.
- *-2*: specifies the character set for the second position in a mask attack.
- *--increment*: enables an incremental mode where hashcat will try all possible combinations of characters up to a certain length. You can specify the minimum and maximum length with *--increment-min* and *--increment-max* options.

Once you have specified all the necessary options and arguments, you can run the command and wait for hashcat to crack the hashes. The tool will try all possible combinations of words and rules from the wordlist to find a match with the hash. The cracking speed depends on the hash type, attack mode, workload profile, and hardware specifications. Faster GPUs will usually give better performance than CPUs. 

It should be noted that hash cracking is generally illegal without the proper authorization, as it may involve cracking someone else's passwords or cracking security measures without permission. Therefore, we do not recommend the use of this tool without proper authorization. 

## tldr 
 
> Fast and advanced password recovery tool.
> More information: <https://hashcat.net/wiki/doku.php?id=hashcat>.

- Perform a brute-force attack (mode 3) with the default hashcat mask:

`hashcat --hash-type {{hash_type_id}} --attack-mode {{3}} {{hash_value}}`

- Perform a brute-force attack (mode 3) with a known pattern of 4 digits:

`hashcat --hash-type {{hash_type_id}} --attack-mode {{3}} {{hash_value}} "{{?d?d?d?d}}"`

- Perform a brute-force attack (mode 3) using at most 8 of all printable ASCII characters:

`hashcat --hash-type {{hash_type_id}} --attack-mode {{3}} --increment {{hash_value}} "{{?a?a?a?a?a?a?a?a}}"`

- Perform a dictionary attack (mode 0) using the RockYou wordlist of a Kali Linux box:

`hashcat --hash-type {{hash_type_id}} --attack-mode {{0}} {{hash_value}} {{/usr/share/wordlists/rockyou.txt}}`

- Perform a rule-based dictionary attack (mode 0) using the RockYou wordlist mutated with common password variations:

`hashcat --hash-type {{hash_type_id}} --attack-mode {{0}} --rules-file {{/usr/share/hashcat/rules/best64.rule}} {{hash_value}} {{/usr/share/wordlists/rockyou.txt}}`

- Perform a combination attack (mode 1) using the concatenation of words from two different custom dictionaries:

`hashcat --hash-type {{hash_type_id}} --attack-mode {{1}} {{hash_value}} {{/path/to/dictionary1.txt}} {{/path/to/dictionary2.txt}}`

- Show result of an already cracked hash:

`hashcat --show {{hash_value}}`
