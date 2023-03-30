# testssl 
## chatgpt 
testssl is a command-line tool used for testing SSL/TLS encryption on websites, servers, and other network services. It is a free and open-source tool that is widely used by web developers, security researchers, system administrators, and penetration testers.

The tool is designed to check the SSL/TLS configuration of a website or a server for potential vulnerabilities and weaknesses. It helps to detect various security issues such as weak ciphers, insecure protocols, and vulnerable SSL certificates. With testssl, users can get a detailed report of the security status of a website or server's SSL/TLS encryption.

The testssl command requires the user to specify the target website or server to be tested. After running the command, the tool starts scanning the server for potential vulnerabilities, and then displays a detailed report of the test results. The report includes information about the SSL configuration, the cipher strength, SSL versions supported, and any vulnerabilities detected.

In summary, the testssl command is a powerful tool for testing the security of SSL/TLS encryption on websites and servers. It helps to identify potential vulnerabilities and weaknesses in the SSL configuration, and provides a comprehensive report of the test results. 

## tldr 
 
> Check SSL/TLS protocols and ciphers supported by a server.
> More information: <https://testssl.sh/>.

- Test a server (run every check) on port 443:

`testssl {{example.com}}`

- Test a different port:

`testssl {{example.com:465}}`

- Only check available protocols:

`testssl --protocols {{example.com}}`

- Only check vulnerabilities:

`testssl --vulnerable {{example.com}}`

- Only check HTTP security headers:

`testssl --headers {{example.com}}`
