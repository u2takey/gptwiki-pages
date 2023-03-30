# ldapsearch 
## chatgpt 
The ldapsearch command is used to search for information in a Lightweight Directory Access Protocol (LDAP) directory. It allows you to retrieve information from the directory and display the results on the command-line interface.

The basic syntax of the ldapsearch command is:

```
ldapsearch [options] [search filter] [attributes]
```

The options specify the configuration settings for connecting to the LDAP server, such as server address, port number, username, and password. The search filter and attributes specify what information should be retrieved from the directory.

Some common options include:

- -H: specifies the LDAP server URL
- -D: specifies the username to authenticate with the LDAP server
- -w: specifies the password to authenticate with the LDAP server
- -b: specifies the search base, which is the starting point of the search in the directory tree
- -s: specifies the scope of the search (one level, subtree, or base)
- -x: specifies to use simple authentication instead of SASL authentication

The search filter is used to specify the search criteria for the information you want to retrieve from the directory. It is written in a specific syntax called LDAP filter syntax. For example, to search for all users with the last name "Smith", the filter would be:

```
(&(objectClass=person)(sn=Smith))
```

The attributes parameter specifies the attributes or fields that you want to retrieve for the search results. For example, to retrieve the first name, last name, and email address of all users, the attributes would be:

```
dn givenName sn mail
```

When you execute the ldapsearch command with the appropriate options, search filter, and attributes, it will connect to the LDAP server, search for the information that matches the specified criteria, and display the results. The results are displayed in LDIF format, which is a standardized way of representing directory information in plain text. The LDIF format includes entries for each result, with attribute names and values listed for each entry. 

## tldr 
 
> CLI utility for querying an LDAP directory.
> More information: <https://docs.ldap.com/ldap-sdk/docs/tool-usages/ldapsearch.html>.

- Query an LDAP server for all items that are a member of the given group and return the object's displayName value:

`ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} -b {{base_ou}} '{{memberOf=group1}}' displayName`

- Query an LDAP server with a no-newline password file for all items that are a member of the given group and return the object's displayName value:

`ldapsearch -D '{{admin_DN}}' -y '{{password_file}}' -h {{ldap_host}} -b {{base_ou}} '{{memberOf=group1}}' displayName`

- Return 5 items that match the given filter:

`ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} -b {{base_ou}} '{{memberOf=group1}}' -z 5 displayName`

- Wait up to 7 seconds for a response:

`ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} -b {{base_ou}} '{{memberOf=group1}}' -l 7 displayName`

- Invert the filter:

`ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} -b {{base_ou}} '(!(memberOf={{group1}}))' displayName`

- Return all items that are part of multiple groups, returning the display name for each item:

`ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} '(&({{memberOf=group1}})({{memberOf=group2}})({{memberOf=group3}}))' "displayName"`

- Return all items that are members of at least 1 of the specified groups:

`ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} '(|({{memberOf=group1}})({{memberOf=group1}})({{memberOf=group3}}))' displayName`

- Combine multiple boolean logic filters:

`ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} '(&({{memberOf=group1}})({{memberOf=group2}})(!({{memberOf=group3}})))' displayName`
