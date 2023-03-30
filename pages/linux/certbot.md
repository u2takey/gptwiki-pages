# certbot 
## chatgpt 
Certbot is a command-line tool that is used to automate the process of obtaining and renewing SSL/TLS certificates from Let's Encrypt. The command "certbot" is used to start the Certbot application and initiate the process of obtaining and installing SSL/TLS certificates on a web server.

When you run the "certbot" command without any parameters, Certbot will start an interactive mode and ask you a series of questions to identify the domain name for which you want to obtain an SSL/TLS certificate, the type of web server you are using, and the verification method you want to use (HTTP or DNS).

Once you have provided the necessary information, Certbot will automatically request an SSL/TLS certificate from Let's Encrypt and install it on your web server. Certbot also configures your web server to use the new certificate and enables automatic renewal of certificates by setting up a cron job.

Some common parameters that can be used with the "certbot" command include options to specify the domain name or names for which you want to obtain and install a certificate, to specify the location of the web server configuration file, to specify the type of web server you are using, and to specify the verification method to use (HTTP or DNS).

Overall, the "certbot" command is a powerful tool for automating the process of obtaining and renewing SSL/TLS certificates and ensuring the security and integrity of your website. 

## tldr 
 
> The Let's Encrypt Agent for automatically obtaining and renewing TLS certificates.
> Successor to `letsencrypt`.
> More information: <https://certbot.eff.org/docs/using.html>.

- Obtain a new certificate via webroot authorization, but do not install it automatically:

`sudo certbot certonly --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}}`

- Obtain a new certificate via nginx authorization, installing the new certificate automatically:

`sudo certbot --nginx --domain {{subdomain.example.com}}`

- Obtain a new certificate via apache authorization, installing the new certificate automatically:

`sudo certbot --apache --domain {{subdomain.example.com}}`

- Renew all Let's Encrypt certificates that expire in 30 days or less (don't forget to restart any servers that use them afterwards):

`sudo certbot renew`

- Simulate the obtaining of a new certificate, but don't actually save any new certificates to disk:

`sudo certbot --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}} --dry-run`

- Obtain an untrusted test certificate instead:

`sudo certbot --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}} --test-cert`
