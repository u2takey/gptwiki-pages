# authconfig 
## chatgpt 
The `authconfig` command is used in Linux to configure authentication and identity services on a system. 

It allows you to enable or disable various authentication methods, such as local passwords, LDAP, NIS, Kerberos, or smart cards. You can also configure various password policies, such as minimum length, complexity requirements, and password expiration.

The `authconfig` command can be used to manage authentication-related services, such as:

1. Configuring authentication settings for users and groups
2. Enabling LDAP authentication
3. Configuring Kerberos authentication
4. Configuring Network Information Service (NIS)
5. Configuring the System Security Services Daemon (SSSD)

When you run the command, you can specify various options to configure different authentication settings. For example, you can use the `--enableldap` option to enable LDAP authentication, or the `--disablesmartcard` option to disable smart card authentication.

Overall, `authconfig` is an important command for system administrators who want to configure the authentication settings of Linux systems in their environment. 

## tldr 
 
> A CLI interface for configuring system authentication resources.
> More information: <https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/system-level_authentication_guide/authconfig-install>.

- Display the current configuration (or dry run):

`authconfig --test`

- Configure the server to use a different password hashing algorithm:

`authconfig --update --passalgo={{algorithm}}`

- Enable LDAP authentication:

`authconfig --update --enableldapauth`

- Disable LDAP authentication:

`authconfig --update --disableldapauth`

- Enable Network Information Service (NIS):

`authconfig --update --enablenis`

- Enable Kerberos:

`authconfig --update --enablekrb5`

- Enable Winbind (Active Directory) authentication:

`authconfig --update --enablewinbindauth`

- Enable local authorization:

`authconfig --update --enablelocauthorize`
