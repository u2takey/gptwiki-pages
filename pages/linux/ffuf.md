# ffuf 
## chatgpt 
ffuf is a popular command-line tool used for fuzzing web applications. It's designed to be fast and flexible, and can be used to discover SQL injections, XSS vulnerabilities, and other web vulnerabilities.

The command is structured as follows:

```
ffuf [flags] -u <url> -w <wordlist> -c -v
```

Here's what each part of the command means:

- `ffuf`: This is the command used to run the ffuf tool.
- `[flags]`: ffuf comes with several optional flags that can be used to customize the tool's behavior. For example, `-w` specifies the wordlist to use for fuzzing, `-ic` makes the tool case-insensitive, and `-mc all` specifies that all responses should be shown, even those without matches.
- `-u <url>`: This specifies the target URL to fuzz. You can include placeholders in the URL that will be replaced with payload strings from the wordlist. For example, `https://example.com/page.php?id=FUZZ` would replace `FUZZ` with each payload in the wordlist.
- `-w <wordlist>`: This specifies the wordlist of payloads to use for fuzzing. Payloads should be separated by new lines.
- `-c`: This specifies that ffuf should exit on the first successful match.
- `-v`: This specifies that ffuf should output verbose information about its progress.

When run, ffuf will use the provided wordlist to fuzz the target URL, replacing each payload string in the wordlist with the `FUZZ` placeholder in the target URL. It will then send each modified URL with the specified HTTP method (defaults to GET) and check the response for matches based on the status code, length or regular expressions. If a match is found, ffuf will print the URL that resulted in the match. 

## tldr 
 
> Subdomain and directory discovery tool.
> More information: <https://github.com/ffuf/ffuf>.

- Discover directories using a [w]ordlist on a target [u]rl with [c]olorized and [v]erbose output:

`ffuf -w {{path/to/wordlist}} -u {{https://target/FUZZ}} -c -v`

- Fuzz host-[H]eaders with a host file on a target website and [m]atch HTTP 200 [c]ode responses:

`ffuf -w {{hosts.txt}} -u {{https://example.org}} -H "{{Host: FUZZ}}" -mc {{200}}`

- Discover directories using a [w]ordlist on a target website with a max individual job time of 60 seconds and recursion discovery depth of 2 levels:

`ffuf -w {{path/to/wordlist}} -u {{https://target/FUZZ}} -maxtime-job {{60}} -recursion -recursion-depth {{2}}`

- Fuzz GET parameter on a target website and [f]ilter out message [s]ize response of 4242 bytes:

`ffuf -w {{path/to/param_names.txt}} -u {{https://target/script.php?FUZZ=test_value}} -fs {{4242}}`

- Fuzz POST method with POST [d]ata of password on a target website and [f]ilter out HTTP response [c]ode 401:

`ffuf -w {{path/to/postdata.txt}} -X {{POST}} -d "{{username=admin\&password=FUZZ}}" -u {{https://target/login.php}} -fc {{401}}`

- Discover subdomains using a subdomain list on a target website:

`ffuf -w {{subdomains.txt}} -u {{https://website.com}} -H "{{Host: FUZZ.website.com}}"`
