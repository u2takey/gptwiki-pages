# redshift 
## chatgpt 
The redshift command is a tool available on Linux and Unix-like systems that adjusts the color temperature of the display. 

The color temperature of a display refers to the color of the light emitted by the screen. Displays are commonly calibrated to have a cool or blueish color temperature, which can cause eye strain and disrupt sleep patterns, particularly when used at night.

The redshift command alters the color temperature of the monitor to make it warmer or more reddish, which can help to reduce eye strain and improve sleep.

The basic syntax of the redshift command is:

`redshift [options]`

The options that can be used with the redshift command include:

- `-l LAT:LON`: changes the location from which the color temperature calculations are based on. LAT and LON represent latitude and longitude values respectively.
- `-t DAY:NIGHT`: sets the transition time between the color temperature during the day and the one that applies during the night. 
- `-r`: resets the color temperature to its default settings. 

By adjusting the color temperature of the display via the redshift command, it can help to reduce eyestrain, minimize exposure to blue light, prevent disruption of sleep patterns, and cause less discomfort when working for long hours at a computer screen. 

## tldr 
 
> Adjust the color temperature of your screen according to your surroundings.
> More information: <http://jonls.dk/redshift>.

- Turn on Redshift with 5700K temperature during day and 3600K at night:

`redshift -t {{5700}}:{{3600}}`

- Turn on Redshift with a manually specified custom location:

`redshift -l {{latitude}}:{{longitude}}`

- Turn on Redshift with 70% screen brightness during day and 40% brightness at night:

`redshift -b {{0.7}}:{{0.4}}`

- Turn on Redshift with custom gamma levels (between 0 and 1):

`redshift -g {{red}}:{{green}}:{{blue}}`

- Turn on Redshift with a constant unchanging color temperature:

`redshift -O {{temperature}}`
