# enum4linux 
## chatgpt 
The enum4linux command is a tool used for enumerating information from Windows and Samba systems. The term "enum" means to enumerate, which refers to the process of mapping out a system to identify all its available resources, access points, and vulnerabilities. The four in the command name refers to the four modes of operation the tool can perform: 

1. User Listing: enum4linux can retrieve a list of users and their associated attributes, such as User ID (UID), Group ID (GID), and home directory. This can be useful for identifying potential targets for further exploitation.

2. Share Enumeration: The command can also retrieve information about the shares available on a target system, including their names, permissions, and contents. This information can be used to identify sensitive files or directories that may have been exposed or misconfigured.

3. Password Policy Retrieval: enum4linux can also retrieve the password policy settings for a target system, which can be used to identify weak passwords, expired password policies, and other vulnerabilities related to authentication.

4. Group Enumeration: Finally, the command can also retrieve a list of groups and their associated attributes, including their Group ID (GID), members, and their associated permissions. This information can be useful in identifying high-privilege groups that may have access to sensitive resources.

Overall, enum4linux is a useful tool for identifying potential vulnerabilities within Windows and Samba systems by enumerating available resources and user data. 

## tldr 
 
> Tool for enumerating Windows and Samba information from remote systems.
> More information: <https://labs.portcullis.co.uk/tools/enum4linux/>.

- Try to enumerate using all methods:

`enum4linux -a {{remote_host}}`

- Enumerate using given login credentials:

`enum4linux -u {{user_name}} -p {{password}} {{remote_host}}`

- List usernames from a given host:

`enum4linux -U {{remote_host}}`

- List shares:

`enum4linux -S {{remote_host}}`

- Get OS information:

`enum4linux -o {{remote_host}}`
