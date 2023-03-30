# sqlmap 
## chatgpt 
SQLMap is an open-source command-line tool developed in Python that helps penetration testers and security researchers identify and exploit SQL injection vulnerabilities in web applications.

The syntax of the SQLMap command is as follows:

```
sqlmap [options]
```

Here, `[options]` stands for the various command-line options available within SQLMap. Some common options used in SQLMap are:

- `-u`: specifies the target URL to be scanned for SQL injection vulnerabilities.
- `-d`: specifies the target database to be scanned for SQL injection vulnerabilities.
- `-o`: specifies the output file to store the results of the scan.
- `-v`: displays verbose output during the scan.
- `--threads`: specifies the number of threads used for parallel scanning.
- `--level`: specifies the level of detection to be performed by SQLMap.
- `--risk`: specifies the risk level of detection to be performed by SQLMap.
- `--batch`: runs SQLMap in batch mode, without requiring user interaction.

Once the appropriate options have been specified, SQLMap will begin scanning the target for SQL injection vulnerabilities. The tool automatically tries multiple SQL injection techniques to identify vulnerabilities, and can even use various evasion techniques to bypass web application firewall (WAF) defenses.

After identifying a vulnerability, SQLMap provides several options for exploiting it, such as dumping the database, extracting sensitive information, or executing arbitrary SQL commands on the target. It also supports various features like cookie handling, custom headers, and session customization to ensure successful exploitation. 

## tldr 
 
> Detect and exploit SQL injection flaws.
> More information: <https://sqlmap.org>.

- Run sqlmap against a single target URL:

`python sqlmap.py -u "{{http://www.target.com/vuln.php?id=1}}"`

- Send data in a POST request (`--data` implies POST request):

`python sqlmap.py -u "{{http://www.target.com/vuln.php}}" --data="{{id=1}}"`

- Change the parameter delimiter (& is the default):

`python sqlmap.py -u "{{http://www.target.com/vuln.php}}" --data="{{query=foobar;id=1}}" --param-del="{{;}}"`

- Select a random `User-Agent` from `./txt/user-agents.txt` and use it:

`python sqlmap.py -u "{{http://www.target.com/vuln.php}}" --random-agent`

- Provide user credentials for HTTP protocol authentication:

`python sqlmap.py -u "{{http://www.target.com/vuln.php}}" --auth-type {{Basic}} --auth-cred "{{testuser:testpass}}"`
