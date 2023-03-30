# chfn 
## chatgpt 
The "chfn" command stands for "change finger information." It is mainly used in the Unix and Linux operating systems to modify the finger information of a user. 

When a user account is created in Unix or Linux, a set of information is associated with that account, including full name, office number, office phone, and home phone. This information can be displayed using the "finger" command.

The "chfn" command allows a user or system administrator to modify this information. It can be used with the following syntax:

chfn [options] [username]

The most common options used with the "chfn" command are as follows:

-f "full name": This option allows the user or administrator to change the full name associated with the account.

-r "room number": This option is used to change the office or room number associated with the account.

-w "work phone number": This option is used to change the work phone number associated with the account.

-h "home phone number": This option is used to change the home phone number associated with the account.

Once the user or administrator makes the desired changes, the new finger information can be viewed using the "finger" command. The command is very useful for updating user account details and can be used to provide more accurate, up-to-date information about users in a Unix or Linux system. 

## tldr 
 
> Update `finger` info for a user.
> More information: <https://manned.org/chfn>.

- Update a user's "Name" field in the output of `finger`:

`chfn -f {{new_display_name}} {{username}}`

- Update a user's "Office Room Number" field for the output of `finger`:

`chfn -o {{new_office_room_number}} {{username}}`

- Update a user's "Office Phone Number" field for the output of `finger`:

`chfn -p {{new_office_telephone_number}} {{username}}`

- Update a user's "Home Phone Number" field for the output of `finger`:

`chfn -h {{new_home_telephone_number}} {{username}}`
