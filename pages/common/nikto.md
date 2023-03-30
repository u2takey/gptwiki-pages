# nikto 
## chatgpt 
Nikto is an open-source web server vulnerability scanner. It helps in identifying various vulnerabilities present in a web server or a website. Here are the details of the Nikto command:

Usage syntax: `nikto -h <target_website_URL>`

Where, `-h` option specifies the target website URL.

After executing the command, Nikto scans the target website and displays the results on the screen. It shows information like server type, open ports, software versions, and vulnerabilities present in the website.

Nikto has many command-line options that can be used to customize the scan as per the need. Some of the commonly used options are:

- `-F`: This option allows to specify a custom file containing a list of target URLs or IP addresses.

- `-output`: This option allows to save the scan report in a specific format like HTML, CSV, XML, etc.

- `-C`: This option allows to specify a custom configuration file to use for the scan.

- `-ssl`: This option allows to enable the SSL scan for HTTPS websites.

- `-Tuning`: This option allows to specify the scan tuning parameters, which can be used to optimize the scan speed and accuracy.

Overall, Nikto is a powerful and useful tool for identifying vulnerabilities in web servers and websites. 

## tldr 
 
> Web server scanner which performs tests against web servers for multiple items.
> More information: <https://cirt.net/Nikto2>.

- Perform a basic Nikto scan against a target host:

`perl nikto.pl -h {{192.168.0.1}}`

- Specify the port number when performing a basic scan:

`perl nikto.pl -h {{192.168.0.1}} -p {{443}}`

- Scan ports and protocols with full URL syntax:

`perl nikto.pl -h {{https://192.168.0.1:443/}}`

- Scan multiple ports in the same scanning session:

`perl nikto.pl -h {{192.168.0.1}} -p {{80,88,443}}`

- Update to the latest plugins and databases:

`perl nikto.pl -update`
