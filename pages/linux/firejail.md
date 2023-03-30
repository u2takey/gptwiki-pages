# firejail 
## chatgpt 
Firejail is a Linux security tool that is designed to protect the system by limiting the access of an application to the rest of the system. The command `firejail` is used to launch a command or an application in a sandboxed environment using Firejail.

The syntax of the `firejail` command is as follows:

```
firejail [options] application
```

Here, `options` are the various configuration options that can be used to customize the behavior of the Firejail sandbox. Some of the commonly used options include:

- `--private`: This option makes sure that the application is launched in a new mount namespace with a private /tmp directory.

- `--noprofile`: This option disables the profile-based sandboxing, which is useful when there is no profile available for the application.

- `--net=none`: This option disables networking for the application inside the sandbox.

After the options, we need to specify the `application` that we want to launch in the sandbox. For example:

```
firejail --private firefox
```

This command will launch the Firefox browser in a sandboxed environment with a private /tmp directory.

Firejail offers a wide range of functionality for sandboxing applications, such as restricting network access, limiting access to files, and preventing the application from spawning other processes. By running applications in a sandbox, it is possible to reduce the attack surface of the system and improve its overall security. 

## tldr 
 
> Securely sandboxes processes to containers using built-in Linux capabilities.
> More information: <https://manned.org/firejail>.

- Integrate firejail with your desktop environment:

`sudo firecfg`

- Open a restricted Mozilla Firefox:

`firejail {{firefox}}`

- Start a restricted Apache server on a known interface and address:

`firejail --net={{eth0}} --ip={{192.168.1.244}} {{/etc/init.d/apache2}} {{start}}`

- List running sandboxes:

`firejail --list`

- List network activity from running sandboxes:

`firejail --netstats`

- Shutdown a running sandbox:

`firejail --shutdown={{7777}}`
