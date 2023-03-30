# swaks 
## chatgpt 
Swaks is a command line utility for sending emails. The name stands for "Swiss Army Knife for SMTP". Swaks can be used to test SMTP servers, check email addresses, and send emails to test email systems. 

Here is the basic syntax for the Swaks command:

`swaks [OPTIONS]`

Some of the most commonly used options are:

- `-f, --from`: Specifies the sender of the email.
- `-t, --to`: Specifies the recipient of the email.
- `-s, --server`: Specifies the SMTP server to use for sending the email.
- `-p, --port`: Specifies the port number for the SMTP server.
- `-auth, --auth`: Enables authentication for SMTP.

Here is an example of how to use Swaks to send a test email:

`swaks --to user@example.com --from admin@example.com --server smtp.example.com`

This command will send an email to user@example.com from admin@example.com using the SMTP server smtp.example.com. 

Overall, Swaks can be a useful tool for testing and troubleshooting email systems. 

## tldr 
 
> Swiss Army Knife SMTP, the all-purpose SMTP transaction tester.
> More information: <https://github.com/jetmore/swaks/blob/develop/doc/base.pod>.

- Deliver a standard test email to `user@example.com` on port 25 of `test-server.example.net`:

`swaks --to {{user@example.com}} --server {{test-server.example.net}}`

- Deliver a standard test email, requiring CRAM-MD5 authentication as user `me@example.com`. An "X-Test" header will be added to the email body:

`swaks --to {{user@example.com}} --from {{me@example.com}} --auth {{CRAM-MD5}} --auth-user {{me@example.com}} --header-X-Test "{{test_email}}"`

- Test a virus scanner using EICAR in an attachment. Don't show the message DATA part:

`swaks -t {{user@example.com}} --attach - --server {{test-server.example.com}} --suppress-data {{path/to/eicar.txt}}`

- Test a spam scanner using GTUBE in the body of an email, routed via the MX records for `example.com`:

`swaks --to {{user@example.com}} --body {{path/to/gtube_file}}`

- Deliver a standard test email to `user@example.com` using the LMTP protocol via a UNIX domain socket file:

`swaks --to {{user@example.com}} --socket {{/var/lda.sock}} --protocol {{LMTP}}`
