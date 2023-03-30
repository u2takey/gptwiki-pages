# chpasswd 
## chatgpt 
The "chpasswd" command is used to change the password of a user account on a Linux or Unix operating system. Here's how the command works:

Syntax:
chpasswd [options] file

Where,
options: These are optional arguments that modify the behavior of the command. Some common options include -e, -c, -s, -m, -u, -T, -s, and -D. 
file : This is the name of the file that contains the list of username and password pairs that the "chpasswd" command will read from, this file must be in a specific format with colon separated list of username and password.


The "chpasswd" command reads a list of username and encrypted password pairs from a specified file, then replaces the password of the specified user account with the new one.

The password should be encrypted or hashed in the file. You can use the "mkpasswd" command to generate an encrypted or hashed password.

Here's an example of how to use the "chpasswd" command to change the password of a user named "John" with password "oldpassword" to a new password "newpassword", in one command:

echo "John:newpassword" | chpasswd

In this example, we're piping the output of the echo command (which creates a string "John:newpassword") to the chpasswd command. The chpasswd command then reads the string and replaces the password for the user "John" with "newpassword".

Note: The use of plain text password is not recommended as it poses a security threat. The passwords should always be encrypted or hashed using the appropriate algorithms. 

## tldr 
 
> Change the passwords for multiple users by using `stdin`.
> More information: <https://manned.org/chpasswd.8>.

- Change the password for a specific user:

`printf "{{username}}:{{new_password}}" | sudo chpasswd`

- Change the passwords for multiple users (The input text must not contain any spaces.):

`printf "{{username_1}}:{{new_password_1}}\n{{username_2}}:{{new_password_2}}" | sudo chpasswd`

- Change the password for a specific user, and specify it in encrypted form:

`printf "{{username}}:{{new_encrypted_password}}" | sudo chpasswd --encrypted`

- Change the password for a specific user, and use a specific encryption for the stored password:

`printf "{{username}}:{{new_password}}" | sudo chpasswd --crypt-method {{NONE|DES|MD5|SHA256|SHA512}}`
