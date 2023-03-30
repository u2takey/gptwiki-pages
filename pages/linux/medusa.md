# Medusa 
## chatgpt 
Medusa is a command-line tool for performing brute-force attacks against a variety of different network protocols. It is designed to be highly configurable and feature-rich, allowing users to customize the attack methodology to suit their needs.

Medusa is capable of performing attacks against a variety of different services, including FTP, SSH, Telnet, HTTP, HTTPS, and more. It uses a variety of different attack methods to try and gain access to the target system, including dictionary attacks, brute-force attacks, and custom attacks.

One of the key features of Medusa is its ability to handle multiple targets and protocols simultaneously. This makes it a powerful tool for penetration testers and security researchers who need to test a variety of different systems and protocols.

In order to use Medusa, users must specify the target system and the protocol they want to attack. They can then configure a variety of different settings, such as the attack method, the credentials to use, and the number of connections to make.

Once the attack is launched, Medusa will attempt to gain access to the target system by brute-forcing its way through different credential combinations. If successful, the user will be able to gain access to the target system and perform whatever actions are necessary for their testing purposes.

Overall, Medusa is a powerful and flexible tool that can be used to test the security of a variety of different systems and protocols. However, it should only be used by experienced users who understand the risks and limitations of brute-force attacks. 

## tldr 
 
> A modular and parallel login brute-forcer for a variety of protocols.
> More information: <https://manned.org/medusa>.

- Execute brute force against an FTP server using a file containing usernames and a file containing passwords:

`medusa -M ftp -h host -U {{path/to/username_file}} -P {{path/to/password_file}}`

- Execute a login attempt against an HTTP server using the username, password and user-agent specified:

`medusa -M HTTP -h host -u {{username}} -p {{password}} -m USER-AGENT:"{{Agent}}"`

- Execute a brute force against a MySQL server using a file containing usernames and a hash:

`medusa -M mysql -h host -U {{path/to/username_file}} -p {{hash}} -m PASS:HASH`

- Execute a brute force against a list of SMB servers using a username and a pwdump file:

`medusa -M smbnt -H {{path/to/hosts_file}} -C {{path/to/pwdump_file}} -u {{username}} -m PASS:HASH`
