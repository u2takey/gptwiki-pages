# pasuspender 
## chatgpt 
The "pasuspender" command is used to temporarily suspend the PulseAudio sound server, which may be required in some cases where the sound device is not properly detected or configured. When this command is executed, any PulseAudio-enabled application that is currently running will be redirected to the ALSA (Advanced Linux Sound Architecture) sound system instead. This can help to troubleshoot and debug problems that are related to PulseAudio, such as audio stuttering, crackling, or other sound issues.

Here's how the command works:

1. Open the terminal window on your Linux system
2. Type in the following command: "pasuspender [application name]", where [application name] is the name of the application that you want to suspend PulseAudio for
3. Hit the "Enter" key to execute the command
4. If the application is currently running, you should see a message that it has been suspended
5. Test the sound on your system to verify that it is working correctly with the ALSA sound system

Note that this command only temporarily suspends PulseAudio- it will automatically restart itself once the application that was suspended is closed or terminated. If you want to permanently disable PulseAudio, you will need to modify your system's configuration files or use an alternative sound system. 

## tldr 
 
> Temporarily suspends `pulseaudio` while another command is running to allow access to alsa.
> More information: <https://manned.org/pasuspender>.

- Suspend PulseAudio while running `jackd`:

`pasuspender -- {{jackd -d alsa --device hw:0}}`
