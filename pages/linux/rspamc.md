# rspamc 
## chatgpt 
The "rspamc" command is a command-line utility tool for interacting with the Rspamd daemon. Rspamd is an advanced spam filtering system that uses various techniques and algorithms to detect and filter out unwanted emails.

The rspamc command allows users to perform various tasks and operations such as checking the status of the Rspamd daemon, submitting messages for spam filtering, extracting statistics, managing blacklists and whitelists, and more.

Here's a brief overview of some common usage scenarios and options for the rspamc command:

1. Check the status of the Rspamd daemon:

To check if the Rspamd daemon is running and responsive, you can run the following command:

```rspamc ping```

If everything is working correctly, you should receive a "pong" response indicating that the daemon is up and running.

2. Submit a message for spam filtering:

To send a message to Rspamd for spam filtering, you can use the following command:

```rspamc learn_spam < /path/to/message```

This will submit the message for processing and update the spam scoring system accordingly. If the message is determined to be spam, it will be automatically marked as such for future filtering.

3. Extract statistics:

To extract various statistics and performance metrics from the Rspamd daemon, you can use the following command:

```rspamc stat```

This will show a summary of various statistics such as the number of processed messages, average scan time, and more.

Overall, the rspamc command is a powerful tool for managing and interacting with the Rspamd spam filtering system. By using this command, you can streamline your spam filtering process and ensure that your email system is protected from unwanted spam and phishing attacks. 

## tldr 
 
> Command-line client for rspamd servers.
> More information: <https://manned.org/rspamc>.

- Train the bayesian filter to recognise an email as spam:

`rspamc learn_spam {{path/to/email_file}}`

- Train the bayesian filter to recognise an email as ham:

`rspamc learn_ham {{path/to/email_file}}`

- Generate a manual report on an email:

`rspamc symbols {{path/to/email_file}}`

- Show server statistics:

`rspamc stat`
