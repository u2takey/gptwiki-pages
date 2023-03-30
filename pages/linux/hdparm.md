# hdparm 
## chatgpt 
The "hdparm" command is a Linux utility that allows users to view and change settings related to a hard disk drive. Some of the functions that can be performed using this command are:

1. Displaying drive information: The "hdparm -i" command can be used to display information about the hard drive.

2. Changing drive parameters: You can use the "hdparm -p" command to change the hard drive parameters. For example, you can use this command to change the power management settings for your hard drive.

3. Running drive tests: The "hdparm -t" command can be used to run read tests on your hard drive. This can help you detect any performance issues with your drive.

Overall, the "hdparm" command is a useful tool for managing hard disk drives in a Linux environment. It can be used to optimize the performance of your drive and also diagnose and troubleshoot any issues that you may encounter. 

## tldr 
 
> Get and set SATA and IDE hard drive parameters.
> More information: <https://manned.org/hdparm>.

- Request the identification info of a given device:

`sudo hdparm -I /dev/{{device}}`

- Get the Advanced Power Management level:

`sudo hdparm -B /dev/{{device}}`

- Set the Advanced Power Management value (values 1-127 permit spin-down, and values 128-254 do not):

`sudo hdparm -B {{1}} /dev/{{device}}`

- Display the device's current power mode status:

`sudo hdparm -C /dev/{{device}}`

- Force a drive to immediately enter standby mode (usually causes a drive to spin down):

`sudo hdparm -y /dev/{{device}}`

- Put the drive into idle (low-power) mode, also setting its standby timeout:

`sudo hdparm -S {{standby_timeout}} {{device}}`

- Test the read speed of a specific device:

`sudo hdparm -tT {{device}}`
