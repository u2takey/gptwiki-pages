# debsecan 
## chatgpt 
Debsecan is a command-line tool used to scan the Debian GNU/Linux operating system for any known vulnerabilities. It is designed to check for unpatched security flaws in both the Debian operating system and third-party software installed on it.

When you run the debsecan command, it will scan the system's package database to look for any packages that have known vulnerabilities. It does this by querying the Debian Security Tracker, which is a comprehensive database of all known security issues affecting Debian.

The debsecan tool can be used in multiple ways. For example, you can scan the entire system for vulnerabilities or scan only specific packages. You can also specify a date range to check for security issues that were discovered within a specific timeframe.

The output of debsecan includes a summary of the packages that have known vulnerabilities, along with information about which versions are affected and what the severity of the issue is. This information can be used to determine which packages need to be updated to address the vulnerabilities.

Overall, debsecan is an essential tool for ensuring the security of a Debian-based system, as it allows you to proactively identify and patch vulnerabilities before they can be exploited. 

## tldr 
 
> Debian Security Analyzer, a tool to list vulnerabilities on a particular Debian installation.
> More information: <https://gitlab.com/fweimer/debsecan>.

- List vulnerable installed packages on the current host:

`debsecan`

- List vulnerable installed packages of a specific suite:

`debsecan --suite {{release_code_name}}`

- List only fixed vulnerabilities:

`debsecan --suite {{release_code_name}} --only-fixed`

- List only fixed vulnerabilities of unstable ("sid") and mail to root:

`debsecan --suite {{sid}} --only-fixed --format {{report}} --mailto {{root}} --update-history`

- Upgrade vulnerable installed packages:

`sudo apt upgrade $(debsecan --only-fixed --format {{packages}})`
